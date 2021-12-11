# consteval
I will be using this repository to build up a library of compile time evaluated functionality as I learn about constant evaluation in Rust. No guarantees as to the quality of the code but I am a big fan of unit testing and test driven development (or at least test guided development). As such, it's likely that every function or type I make here will have a unit test associated with it to raise confidence in the functionality.

## Rationale ##
Rust has the ability to have the compiler itself run the functions we want in a constant context. The main unit of functionality that can support this is the const function. Const functions in Rust are limited in what they can do as they must be able to run both at compile time and runtime and so we need to find replacement methods to achieve the results that we normally have access to in the standard library.

This is the reason I am looking into constant evaluation as the more we can do at compile time, the less we need to do (and the faster it'll be) at runtime.
