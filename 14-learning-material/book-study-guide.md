# Book study guide

Use reading to improve implemented work: take a short note, challenge it with a counterexample, and make a verifiable change. Do not reproduce the books in the repository. Sources below were checked on 6 October 2026.

## Clean Code by Robert C. Martin

The original edition addresses code readability, naming, functions, comments, errors, boundaries, tests, design and concurrency. Study it through the [craftsmanship exercises](../17-clean-code-and-craftsmanship/), preserving behavior as you refactor.

Pearson also lists a second edition published in 2025 with a changed structure and broader design/architecture and professional-practice coverage. Record your edition in reading notes; do not transfer chapter numbers between editions. The curriculum maps themes, not an assumed edition.

Sources: [original edition publisher contents](https://www.pearson.com/en-us/subject-catalog/p/clean-code-a-handbook-of-agile-software-craftsmanship/P200000009044/9780136083252), [second edition publisher contents](https://www.pearson.com/en-us/subject-catalog/p/clean-code-a-handbook-of-agile-software-craftsmanship-2nd-edition/P200000013239/9780135398579).

## The Clean Coder by Robert C. Martin

This is a distinct book about professional conduct. Its contents include responsibility, commitments, TDD, practice, acceptance tests, testing strategy, time management, estimation, pressure, collaboration, teams and mentoring. The initial curriculum did not make all these explicit.

Apply the themes in [professional practice](../12-professional-practice/), [test-first work](../08-testing-and-quality/tdd-red-green-refactor/), [craftsmanship](../17-clean-code-and-craftsmanship/) and [Senior/Lead engineering](../16-senior-lead-engineering/). Produce an estimate with uncertainty, a risk update, an acceptance scenario and useful review feedback.

Source: [publisher contents](https://www.pearson.com/en-us/subject-catalog/p/Martin-Clean-Coder-The-A-Code-of-Conduct-for-Professional-Programmers/P200000009045?view=educator).

## Clean Architecture by Robert C. Martin

Beyond the familiar layer diagram, the contents cover SOLID, component cohesion/coupling, dependency direction, boundaries, policy, business rules, composition, presenters/humble objects, services and test boundaries. These justify more specific architecture exercises.

Study [clean/hexagonal architecture](../10-architecture-and-system-design/clean-and-hexagonal/), [component principles](../10-architecture-and-system-design/component-cohesion-and-coupling/) and [architecture checks](../10-architecture-and-system-design/architecture-fitness-functions/). Implement a use case whose domain rules can be tested independently of HTTP and persistence; compare the cost with a simpler vertical slice.

Source: [publisher contents](https://www.pearson.com/en-gb/subject-catalog/p/clean-architecture-a-craftsmans-guide-to-software-structure-and-design/P200000009528/9780134494166).

## Domain-Driven Design by Eric Evans

The author describes a framework and vocabulary for design around complex domains. The accompanying reference distinguishes language/modeling, tactical building blocks, strategic contexts and integration, and deeper model refinement. A folder containing entities and repositories alone would not cover that scope.

Use the [six DDD exercises](../10-architecture-and-system-design/domain-driven-design/) to move from business examples to context boundaries, invariant-protecting aggregates and integration. Write a context map, show a model changing after new domain knowledge, and justify where ordinary CRUD is enough.

Sources: [author's DDD resources](https://www.domainlanguage.com/ddd/), [author's reference definitions and patterns](https://www.domainlanguage.com/wp-content/uploads/2016/05/DDD_Reference_2015-03.pdf).

## Suggested reading and practice sequence

1. Clean Code themes alongside a refactoring and TDD exercise.
2. The Clean Coder themes throughout estimation, review and delivery practice.
3. Clean Architecture alongside a runnable backend and architecture checks.
4. DDD alongside inventory/orders with actual business invariants and evolving requirements.

Read selectively around the current project, then revisit the wider books. Compare advice with modern C# idioms and the project constraints; record why an exception makes sense instead of enforcing rules mechanically.
