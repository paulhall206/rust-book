Now that we have proof-of-life on our Rust compiler, let's start with a simple program for a guessing game.
We'll get into
- reading and writing from the terminal
- static and mutable variables
- random number generation
- looping
- type casting
- detecting errors from a library

Starting with ```cargo new guessing_game``` we can then ```cd``` into the guessing_game directory and ```cargo run``` to get things going.  It turns out you need to drop into the new directory as ```cargo``` needs that ```Cargo.toml``` file to be in the current (or parent) directory.

For an old C programmer, Rust has taken the opposite choice on variables.  By default, a C variable is writable.  You have to add ```static``` to keep it read only.  However, Rust made the opposite choice.  You need to add ```mut``` (for mutable or changeable) to write new values into a variable.  When in doubt, Rust makes it safe.

Rust structure is matching braces, just like C. VS Code handles this quite well.

Rust type casting is different.  Instead of allocating a variable of a specific type, Rust can shadow a variable to keep type out of the semantics.  I'm not sure I like that, but here's how it looks.  _Distance_ has two variables in C: a float and an integer but in Rust, _distance_ is shadowed by the types.  My guess is that the float _distance_ has gone out of scope once it's cast to an integer but in C, both values are available.

| C code                        | Rust code|
|-------------------------------|------------------------------|
| float fDistance;              | let mut distance: f32 = 5.0; |
| int iDistance;                |                              |
| iDistance = (int) fDistance;  | let distance: i32 = 5;       |


