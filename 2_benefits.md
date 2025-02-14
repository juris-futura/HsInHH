
## Benefits:

* significant Python code generation (for both implemenation and caller)
* JSON payload safety
* very simple to write UI, UI - Data binding is second to none
* graphic UI designer
* golden tests generation with correct input / output shapes
* type based DI
* static code analysis / compilation warnings
* logic solver integration
* encourages unique types (e.g. naming string scalars)


## Other Functionality Highlights:

* very similar to GraphQL, but adds arrow like atoms that can be manipulated
* static defaulting of JSON (not shown)
* per target deployment replacements (not shown)
* built-in ORM (not shown)
* compilation flags


## Concepts at High Level:

* HKT pattern
* Lambda Calculus / Hindley-Milner (1/2 of LC (application, no abstraction))
* Type based traversals (Optics - traverse "big" Juvo type given "small" Juvo type, statically verify soundness of such traversals)
* DI (invoking atoms, molecules)
* lots of static verification


## Tech at High Level:

* Recursion schemes (Kmett's library)
* Effect Systems / EDSLs
* WS processing with streaming
* ...