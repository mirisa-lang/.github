# The Mirisa Programming Language (early WIP)

Mirisa will be a general-purpose programming language and toolchain for maintaining safe, robust, and optimal software. It will have a formal specification and little to no language changes after release.

It aims to be a safe and expressive yet simple systems programming language. And these will be the main features:

* algebraic effects: it provides a better way to work with effects, so exceptions, generators, async, dependency injection, control over io, etc using just a single simple yet powerful and safe languge feature;
* algebraic coeffects: it provides a better way to work with context, so a borrow checker and lifetimes alternative, features, better work with os-specific apis, safe dynamic scoping, etc. from a single feature;
* refinement types: to reduce the need in runtime checks and enforce way more invariants with types (yeah this isn't that new, but afaik still not that widely used);
* staged metaprogramming like in zig but with typeclasses.

## Status of the project

Well… i am working on a PoC c with algebraic effects and cute syntax to c translator.

### Roadmap:

* finish PoC c with algebraic effects and cute syntax to c translator;
* it's own typechecker with the zero type and maybe a better type for c's void*;
* make variants actual ADTs;
* functions-like handlers (idk how they're actually named);
* self-hosting compiler and vscose (and maybe clion/rustrover) plugin with syntax highliting;
* to be continued…
