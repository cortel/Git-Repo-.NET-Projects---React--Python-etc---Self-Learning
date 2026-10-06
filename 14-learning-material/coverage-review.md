# Curriculum coverage and gap review

The initial repository covered many topics by name but mostly contained generic exercise checklists. The supplied notes add detail, not proof of practical mastery. This review maps the material and official book topic outlines to concrete exercises for an intermediate developer progressing toward Senior and Lead responsibilities.

## What the comparison revealed

| Area | Before this update | Added or strengthened |
| --- | --- | --- |
| Clean Code | General SOLID/refactoring topic | Naming/functions, errors/nullability, smells, dependency boundaries, clean tests and concurrency exercises |
| The Clean Coder | Requirements, estimation and writing folders | Commitments, pressure, sustainable practice, acceptance tests, deliberate practice, mentoring and stakeholder communication |
| TDD | Unit tests were present; test-first process was not explicit | Red/green/refactor lab, acceptance/BDD lab and characterization/test-double lab |
| Clean Architecture | Clean/hexagonal and ADR folders | Component principles, executable dependency checks, use-case boundaries, composition root and independent domain tests |
| DDD | A single general topic folder | Six discovery, strategic modeling, tactical modeling, integration and model-refinement exercises |
| GRASP | Only broad design principles; supplied PDF covers five principles | All nine principles with responsibility-assignment and tradeoff exercises |
| Algorithms | One broad algorithms folder | Sorting/stability and searching/graphs labs tied to supplied comparisons |
| .NET collections and runtime | Generic C#/LINQ and concurrency topics | Operation-specific collection benchmarks, allocation/GC/pooling and DI/decorator checks |
| Legacy ASP.NET | Modern API emphasis | MVC/Razor/jQuery-to-React migration with model binding, async, identity, EF and browser debugging |
| Agentic AI infrastructure | Tool-calling, RAG and model use folders | 16 runtime, persistence, queue, gateway, security, approval, evaluation and operational exercises |
| Senior delivery | Technical topics with generic completion criteria | Capacity design, production ownership, safe migration and design-defense evidence |
| Lead responsibilities | Professional practice topics without leadership exercises | RFC reviews, mentoring, team boundaries, risk communication, technical strategy and delivery metrics |

## Additional depth beyond the four books and supplied notes

The expanded plan also requires security threat models, accessibility, contract compatibility, observability, recovery drills, deployment rollback, cloud cost measurements and AI evaluation. These are curriculum additions for the user's goals, rather than claims that every cited book teaches them.

For advanced distributed work, explicitly test network partitions, duplicate messages, clock/order assumptions, schema evolution, stale caches and partial failure. Existing [architecture](../10-architecture-and-system-design/) and [DevOps](../06-devops-and-cloud/) tracks supply the implementation space; the new [system design exercise](../16-senior-lead-engineering/01-system-design-and-capacity/) requires design and capacity evidence.

## Priority

Use [Start here](../00-roadmap/start-here.md) as the single learning order. The existing folders provide supporting depth. The [curated post review](./curated-links.md) removes repeated resources, classifies optional topics and replaces unusable citation placeholders.

Seniority requires evidence from implementation, changed requirements and collaboration; a reading list alone cannot establish it.

## Review boundaries

The five supplied documents were reviewed directly. The book comparison uses official publisher tables of contents/overviews and Eric Evans' author-provided DDD reference. Full copies of the four commercial books were not supplied; this is a topic-level gap analysis, not a page-by-page audit of every book. Sources and edition handling are in the [book study guide](./book-study-guide.md).
