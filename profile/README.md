# The Mirisa Programming Language (early WIP)

Mirisa will be a general-purpose programming language and toolchain for maintaining safe, robust, and optimal software.

It aims to be a safe and expressive yet simple systems programming language. And these will be the main features:

* algebraic effects: to have exceptions, generators, async, dependency injection, etc using just a single simple yet powerful and safe languge feature;
* refinement types (or maybe even dependent types): to reduce runtime checks and enforce way more (any) invariants with types (yeah this isn't that new, but afaik still not that widely used);
* (algebraic? i don't know much about them…) coeffects: afaik it provides a better way to work with context, so a borrow checker and lifetimes alternative, features, better work with os-specific apis, safe dynamic scoping, etc. from a single feature;

and also:

* HKTs: to make convinient traits to work with containers, generators and so on;
* probably GADTs/CIC/?: to enforce more invariants in data type declarations, they replace ADTs so don't count as more features;
* maybe passing values in generics to make work with arrays and similar things more convinient (if there will be no real dependent types like in agda);
* maybe functions on types (if no deptypes again).

## Status of the project

Well… i am working on a PoC c with algebraic effects and cute syntax to c translator. And after that:

* it's own typechecker with the bottom type and maybe a better type for c's void*;
* make variants actual ADTs;
* rewrite to a more advanced translation technique;
* anonymous functions;
* functions-like handlers (idk how they're actually named);
* more algebraic-effects-related (sub)features?
* genarics;
* traits;
* modules;
* rework references and arrays to be more modern and mirisa-way;
* better mirisa as separate language — c interoperability
* vscose (and maybe clion/rustrover) plugin with syntax highliting;
* self-hosting compiler;
* HKTs;
* formatter;
* lsp;
* llvm codegen;
* it's own optimizations;
* standard library;
* to be continued…
