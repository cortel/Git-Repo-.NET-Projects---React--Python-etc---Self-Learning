# Supplied material catalog

Reviewed 6 October 2026 through DOCX paragraph/table extraction, all 14 PDF pages, the two embedded images in the legacy notes, and a visual check of the PDF code sample. This is a curriculum/content review; the retained files were not reformatted or corrected in place.

| Material | What is present | Curriculum use | Review finding |
| --- | --- | --- | --- |
| [Sorting Algorithms complexity comparision.docx](./supplied-documents/Sorting%20Algorithms%20complexity%20comparision.docx) | Sorting/searching comparisons, complexity, stability, claimed .NET implementations | [Sorting lab](../01-foundations/sorting-and-stability-lab/), [search/graph lab](../01-foundations/searching-and-graphs-lab/) | Useful overview; implementation claims and complexity assumptions need corrections |
| [C# Lead Developer System Design & Architecture .pdf](./supplied-documents/C%23%20Lead%20Developer%20System%20Design%20%26%20Architecture%20.pdf) | System design, load balancing, caching, sharding, persistence models, OSI, async, SOLID, five GRASP principles, selected patterns, DI, LINQ and GC | [Senior/Lead engineering](../16-senior-lead-engineering/), [runtime lab](../02-dotnet-backend/runtime-gc-and-memory/), existing architecture/pattern tracks | Good interview prompts; requires deeper practical evidence and corrections to memory, DI decoration and architecture generalizations |
| [Clean + DDD.docx](./supplied-documents/Clean%20%2B%20DDD.docx) | A short statement of intent to take notes on Clean Code, Clean Architecture and DDD and build projects | [Book guide](./book-study-guide.md), [craftsmanship](../17-clean-code-and-craftsmanship/) | Placeholder, not substantive book coverage |
| [NET Collections Cheat Sheet.docx](./supplied-documents/NET%20Collections%20Cheat%20Sheet.docx) | Mutable, immutable and concurrent collection comparisons, channels and pooling | [Collections lab](../02-dotnet-backend/collections-and-allocation-lab/) | Separate indexing from value lookup and operation-specific removal; verify implementation details |
| [Notes Overall NET Core.docx](./supplied-documents/Notes%20Overall%20NET%20Core.docx) | Historical Visual Studio/Git tips, MVC/Razor/jQuery flows, Identity, EF relationships, browser debugging, JSON and file download examples | [Legacy migration](../02-dotnet-backend/legacy-mvc-and-react-migration/), [EF Core](../02-dotnet-backend/ef-core/), [debugging](../01-foundations/debugging-and-profiling/) | Useful modernization exercises; contains synchronous async waits, inappropriate error status choices and reversed debugger shortcut descriptions |

The source directory also contains a ZIP archive. It was not among the five requested files and was not imported or reviewed.

## How to study these notes

Read the relevant note alongside [technical corrections](./technical-corrections.md), then implement an exercise and record the SDK/runtime version, measurements and tradeoffs. Treat shorthand interview claims as hypotheses to validate, rather than universal design rules.

File identity and integrity are recorded in [manifest.json](./manifest.json). Copies preserve the supplied filenames and bytes.
