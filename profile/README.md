# The Mirisa Programming Language (early WIP)

Mirisa will be a general-purpose programming language and toolchain for maintaining safe, robust, and optimal software. It will have a formal specification and little to no language changes after release.

It aims to be a safe and expressive yet simple systems programming language. And these will be the main features:

* algebraic effects: it provides a better way to work with effects, so exceptions, generators, async, dependency injection, control over io, etc using just a single simple yet powerful and safe languge feature;
* algebraic coeffects: it provides a better way to work with context, so a borrow checker and lifetimes alternative, features, better work with os-specific apis, safe dynamic scoping, etc. from a single feature;
* refinement types: to reduce the need in runtime checks and enforce any invariants with types (yeah this isn't that new, but afaik still not that widely used);
* compiletime dependent types like in zig but with typeclasses and (i hope) HKTs: for metaprogramming.
* GADTs: to enforce more invariants in data type declarations, they replace ADTs so don't count as more features;

## Status of the project

Well… i am working on a PoC c with algebraic effects and cute syntax to c translator.

### Roadmap:

* finish PoC c with algebraic effects and cute syntax to c translator;
* it's own typechecker with the zero type and maybe a better type for c's void*;
* make variants actual ADTs;
* functions-like handlers (idk how they're actually named);
* self-hosting compiler and vscose (and maybe clion/rustrover) plugin with syntax highliting;
* to be continued…

### Open questions:

* memory management model: it must be something safe, automatic and without GC, probably a some kind of coeffects-based approach;
* how expressive should mirisa really be;
* how should basic things be made? eg. should things like native numeric types be included to the language or be expressed using other features like inline asm;
* visibility and shadowing;
* interop with c, zig, rust and other languages;
* actually, like anything is an open question…
