# Process backlog

## Sprint 1

### Goals

- Implement the concept of VM status in Rust | Filippo, Angela
- Define high level API in Scala 3 | Paolo, Leonardo

### Review

In RuFi-core:

- Implemented AST [#15](https://github.com/RustFields/RuFi-core/pull/15)
- Implemented Export [#20](https://github.com/RustFields/RuFi-core/pull/20)
- Configured Semantic Release [#17](https://github.com/RustFields/RuFi-core/pull/17)

In ScaFi-core:

- Implemented Path and Slot [#6](https://github.com/RustFields/ScaFi-core/pull/6)

Started working on reifying Fields

## Sprint 2

### Goals

In RuFi-core:
- Implement Context
- Start the RoundVM implementation

In ScaFi-core:
- Implement Export
- Reify Fields
- Port old RoundVM in Scala 3
- Implement Fields API
- Configure Semantic Release

### Review

In RuFi-core:
- Context is implemented [#22](https://github.com/RustFields/RuFi-core/pull/22)
- The RoundVM implementation has started [#25](https://github.com/RustFields/RuFi-core/pull/25)
- Fixed the behavior of Path [26](https://github.com/RustFields/RuFi-core/pull/26)
- Refactored Context API [#28](https://github.com/RustFields/RuFi-core/pull/28)

In ScaFi-core:
- There were problems during the configuration of Semantic Release
- Fields were reified
- Implemented Export
- Implemented Context

## Sprint 3

### Goals

In RuFi-core:

- Finish RoundVM

In ScaFi-core:

- Start implementing field calculus constructs
- Finish porting RoundVM in Scala 3

### Review

In RuFi-core:

- implemented RoundVM

In ScaFi-core:

- implemented nbr and rep
- decided against implementing RoundVM in Scala for the moment: reason is, we should use our wrapped rust implementation

## Sprint 4

### Goals

In ScaFi Core:

- See if we can refactor the VM, accounting for Fields (may create another alternative project)
- Split Fields codebase into a library

In RuFi-core-wrapper:

- setup Java-Rust project
- Experiment with different solutions: JNI, Wasmer, ScalaNative (may need different projects)

### Review

In ScaFi Core:

- Fields codebase was split into a library

In RuFi-core-wrapper:

- Tested different ways to integrate RuFi in Scala, chose Scala Native
- Built a working example that uses Scala Native and integrates some Rust functions thanks to C interoperability

## Sprint 5

### Goals

In RuFi-core-wrapper:

- Define a Gradle+SBT+Cargo project that integrates RuFi in Scala
- Start the implementation

In ScaFi-core:

- Implement remaining constructs and builtins

In RuFi-core:

- Implement language constructs

In ScaFi-fields:

- Add dependency from ScaFi-core

### Review

In RuFi-core-wrapper:

- SBT+Cargo project has been defined
- Implementation has not started yet due to compatibilty issues

In Scafi-core:

- Implement remaining constructs and builtins

In Rufi-core:

- The language is not yet implemented due to Rust limitations.
- Some solutions has been explored to overcome this issues.

In ScaFi-fields:

- Fix semantic-release

## Sprint 6

### Goals

In RuFi-core-wrapper:

- Start the implementation

In Rufi-core:

- Explore solutions to implement language constructs

In ScaFi-fields:

- Add dependency from ScaFi-core

### Review

In ScaFi-fields:

- Added dependency from ScaFi-core
- Implemented core language constructs

Experiments over code interoperability and language constructs in Rust have revealed serious and complex problems.

## Sprint 7

### Goals

In RuFi-core:

- Change VM APIs to make them immutable
- Implement core language constructs

In ScaFi-core:

- Add TestByRound and TestByEquivalence

In ScaFi-fields:

- Check TestByRound correctness
- Add TestByEquivalence

### Review

In RuFi-core:

- Decided to not make RoundVM immutable
- Implemented core language constructs

In ScaFi-core:

- Added TestByRound and TestByEquivalence

In ScaFi-fields:

- TestByRound works correctly but needs to be expanded
- TestByEquivalence needs to be added

## Sprint 8

### Goals

In RuFi-core:

- Implement TestByRound and TestByEquivalence
- Refactor nest with nestIn and nestOut

In ScaFi-fields:

- Expand TestByRound
- Implement TestByEquivalence

### Review

In RuFi-core:

- Refactored nest with nestIn and nestOut

In ScaFi-fields:

- Expanded TestByRound
- Implemented TestByEquivalence

## Sprint 9

### Goals

In RuFi-core:

- Implement TestByEquivalence