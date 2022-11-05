# JavaScript interview questions

[Contribution guidelines for this project](docs/CONTRIBUTING.md)


1. How JS engine works?

![JS Engine](https://images.ctfassets.net/aq13lwl6616q/3o7Q3edCrVJG9Zzj6VMZ1K/28136a643636dfa04090f3fb5c5467ff/javascript_engine.png)

There are many JS engines typically created by web browser vendors.
All engines are standarized by ECMA or ES.

- Parser - analyzing source code, checking it for errors and breaking into parts
- AST - produces tree, contains structural and content related details
- Interpreter - executes lines of code line by line. It can use different strategies to increase performance. Can parse source code and execute it, translate it, execute precompiled code...
- Compiler - take one language and convert it to different one. ex. Typescript, Babel (from JS to older JS)

In modern engines, the interpreter starts reading the code line by line while the profiler watches for frequently used code and flags then passes is to the compiler to be optimized.
In the end, the JavaScript engine takes the bytecode the interpreter outputs and mixes in the optimized code the compiler outputs and then gives that to the computer. This is called "Just in Time" or JIT Compiler.