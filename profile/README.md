# The Mirisa Programming Language (early WIP)

Mirisa will be a general-purpose systems programming language and toolchain for maintaining safe, robust, and optimal firmware and software. It will have a formal specification and little to no language changes after release.

Why when there is rust/zig/etc? because i want algebraic effects, refinement types and powerful generics with typeclasses and HKTs out of the box in a low-level language like zig. also c-like syntax isn't cute at all!

These will be the main features:

* algebraic effects: it provides a better way to work with effects, so exceptions, generators, async, dependency injection, control over io, etc using just a single simple yet powerful and safe languge feature;
* refinement types: to reduce the need in runtime checks and enforce way more invariants with types;
* powerful generics with typeclasses and HKTs;
* compiletime code execution with type introspection and maybe macros based on first-class typed ast manipulations;
* implicit parameters;
* GADTs: more expressive data type definitions.

## Status of the project

Well… i am working on a proof of concept translator to c/zig/llvm (idk which one for now).

### Roadmap:

* finish PoC translator (with only algebraic effects, modules and most basic functionality);
* make self-hosting compiler and vscode plugin (and maybe for clion/rustrover) with syntax highliting and autocomplete;
* implement other features;
* to be continued…
