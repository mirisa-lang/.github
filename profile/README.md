# The Mirisa Programming Language (early WIP)

Mirisa will be a general-purpose programming language and toolchain for maintaining safe, robust, and optimal software.

It aims to be a very safe and expressive yet simple systems programming language without being a workaround-driven kitchen sink like rust… How? Well… here comes The 3 Most Major Mirisa's Features:

* algebraic effects: to have exceptions, generators, async, dependency injection, etc using just a single simple yet powerful and safe languge feature;
* refinement types: to reduce runtime checks and enforce way more invariants with types (yeah this isn't that new, but afaik still not that widely used);
* coeffects: afaik it provides a better way to work with context, so a borrow checker and lifetimes alternative, features, better work with os-specific apis, safe dynamic scoping, etc. from a single feature.

## Status of the project

Well… i am working on a PoC c with algebraic effects to regular c translator… A snippet of code for it:

```
include stdio

effect Console
    log(*char) unit
end

const msgs: *const *const char = [
    "say gex\n",
    "meow~~~\n"
]

function main() i32 do
    try
        var i: i32 = 0
        while i < 2 do
            log(msgs[i])
            i += 1
        end
    handle Console
        log(msg)
            printf("%s\n", msg)
        end
    end
    return 0
end
```
