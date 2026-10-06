# Technical corrections and qualifications

The five supplied originals remain unchanged. These are separate study notes based on the content review and primary references checked on 6 October 2026. Runtime implementation details are version-sensitive; record a concrete SDK/runtime version in experiments.

## Sorting and searching comparison

The Timsort row attributes it to Array.Sort and List<T>.Sort, including reference-type defaults. Microsoft documents introsort and unstable sorting for these APIs. Replace that mapping in your study notes. [Array.Sort](https://learn.microsoft.com/en-us/dotnet/api/system.array.sort?view=net-10.0), [List.Sort](https://learn.microsoft.com/en-us/dotnet/api/system.collections.generic.list-1.sort?view=net-10.0).

Enumerable.OrderBy promises stable ordering, but that contract does not promise merge sort. Do not infer a fixed internal algorithm from the stability guarantee. PLINQ has its own ordering rules; ordinary parallel queries do not preserve source order by default. [OrderBy contract](https://learn.microsoft.com/en-us/dotnet/api/system.linq.enumerable.orderby?view=net-10.0), [PLINQ ordering](https://learn.microsoft.com/en-us/dotnet/standard/parallel-programming/order-preservation-in-plinq).

Other table entries need explicit assumptions before use: quicksort recursion space depends on partitioning/implementation; stable counting sort commonly needs output storage as well as counts; bucket stability depends on within-bucket ordering; A* bounds depend on graph/search model and heuristic conditions. Treat these as follow-up analysis exercises rather than universal figures. For any table, define n, key range, radix/digit count, and whether output memory is counted.

## Collections cheat sheet

The ImmutableList search column conflates indexed access with searching for an arbitrary value. The runtime's IndexOf iterates until a match; the worst-case value search is linear, despite the tree representation. Remove-by-value similarly includes a search before the indexed removal. This is an inference from the implementation, not an assumption that every tree operation is logarithmic. [IndexOf API](https://learn.microsoft.com/en-us/dotnet/api/system.collections.immutable.immutablelist-1.indexof?view=net-10.0), [runtime implementation](https://github.com/dotnet/runtime/blob/main/src/libraries/System.Collections.Immutable/src/System/Collections/Immutable/ImmutableList_1.Node.cs).

The ImmutableDictionary note calls it a hash-array mapped trie. The reviewed .NET runtime implementation stores hash buckets in a SortedInt32KeyNode tree; do not use another language's immutable-map implementation as its description. [runtime source](https://github.com/dotnet/runtime/blob/main/src/libraries/System.Collections.Immutable/src/System/Collections/Immutable/ImmutableDictionary_2.cs).

PriorityQueue removal needs an operation name. Dequeue is different from removing an arbitrary element. The documented Remove method scans linearly; the sheet's RemoveById name is not that BCL API. Check availability on your target framework. [PriorityQueue.Remove](https://learn.microsoft.com/en-us/dotnet/api/system.collections.generic.priorityqueue-2.remove?view=net-10.0).

Interpret Ordered as a defined policy: Stack is LIFO and Queue is FIFO; neither is an unordered bag merely because it is not sorted. Immutable collections do not make compound updates to a shared variable automatically atomic, and ArrayPool is a buffer-management facility, not a searchable collection API. The [collections lab](../02-dotnet-backend/collections-and-allocation-lab/) separates these questions and requires measurements.

## C# Lead Developer system design PDF

Page 14 states that value types live on the stack without GC overhead. Value types can also be inline in heap-resident objects/arrays and can be boxed into allocated objects. Learn value/reference semantics separately from storage location. [class/struct guidance](https://learn.microsoft.com/en-us/dotnet/standard/design-guidelines/choosing-between-class-and-struct), [boxing](https://learn.microsoft.com/en-us/dotnet/csharp/programming-guide/types/boxing-and-unboxing).

Page 10 registers LoggingOrderService as IOrderService while its constructor itself requires IOrderService. With only that shown registration, resolution is circular. Register a separate wrapped concrete service and construct the decorator around it, or use an appropriate decoration mechanism. This finding follows from the shown constructor/registration and DI resolution. Scoped means per scope; an HTTP request is a common scope, not the universal meaning. [DI guidance](https://learn.microsoft.com/en-us/dotnet/core/extensions/dependency-injection/guidelines).

The same page's builder returns its mutable internal product; reusing the builder can mutate a previously returned result. Decide whether Build transfers ownership, copies state, resets the builder or returns an immutable value, and test that choice.

Pages 3-5 generalize high traffic, microservice fault tolerance and SQL/NoSQL consistency. They are useful discussion prompts, not selection rules. High request rates alone do not require microservices or eventual consistency, and service boundaries alone do not ensure isolation. Consistency depends on the specific product and configuration; Cosmos DB, for example, offers multiple levels including strong consistency. [Cosmos DB consistency choices](https://learn.microsoft.com/en-us/azure/cosmos-db/consistency-levels). Test alternatives and use measured requirements in the [capacity exercise](../16-senior-lead-engineering/01-system-design-and-capacity/).

## Historical .NET notes

The sample uses .Result on an asynchronous Identity lookup in a Razor view. Move orchestration to the controller/application layer and await it; avoid blocking async I/O on request paths. [ASP.NET Core best practices](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/best-practices).

The notes first use nonstandard 4001/4002 statuses, then suggest 417/424 for generic invalid login input. These are not appropriate generic validation/authentication codes: 417 concerns an unsatisfied Expect header. Choose a valid status matching the endpoint semantics (such as 400 for invalid input, or 401 for an applicable authentication challenge) and a structured body. Keep authentication messages from revealing whether an account exists. [HTTP semantics](https://www.rfc-editor.org/rfc/rfc9110.html), [ASP.NET error handling](https://learn.microsoft.com/en-us/aspnet/core/web-api/handle-errors).

The debugger notes reverse the common stepping shortcuts. Standard Visual Studio mappings are F10 Step Over, F11 Step Into, Shift+F11 Step Out. Custom keymaps can differ. [debugger navigation](https://learn.microsoft.com/en-us/visualstudio/debugger/navigating-through-code-with-the-debugger).

The file-download sample uses an Excel MIME type for a DOCX. In a new exercise use the correct content type, authorization, controlled file identifiers, and path validation rather than accepting arbitrary client paths. The [migration lab](../02-dotnet-backend/legacy-mvc-and-react-migration/) revisits these examples with synthetic data.

## Clean + DDD note

This file is a placeholder for future book notes. Start with the [book guide](./book-study-guide.md) and turn each useful idea into a code change, a test, a diagram or an architecture decision.
