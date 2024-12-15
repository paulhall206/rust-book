This is the getting started chapter of The Rust Book.
I'm running this through VS Code where the rust-analyzer extension is installed.

# Installing Rust

I'm not sure if the VS Code extension installed the rust tools or if I did that directly.
But ```rustc --version``` works fine in both the VS Code Power Shell Terminal and an separate PS terminal window.

# Hello, World!

The first exercise is Hello World!  That's set up in the projects directory where we create the main.rs file directly.  Rustc is gracious to note that ```println!``` is similar to the ```prinntln!``` misspelling I had.  These error messages are great.

```
> rustc main.rs
> ./main
```
works just great.

# Hello, Cargo!

Now we use the cargo tools to create a standard project directory structure, build the code and run.  It's pretty simple, try:

```
> cargo new hello_cargo
> cargo build
> ./target/debug/hello_cargo.exe
```
We've learned how to install rust, build hello world, and taken first steps with the cargo system.  Cargo has many options, ```cargo help``` will gove you a list.

Here's what we learned:
- ```cargo new project_name```: create the default directory structure and add a hello world program.
- ```cargo build```: build the code using a debug target by default
- ```cargo build --release```: build an optimized target for release
- ```cargo run```: run the debug executable, doing a build if necessary
- ```cargo check```: a quick build but no executable is made.  Use this to check any interim development.

What I'm really looking forward to is learning about ```cargo test``` that executes tests you define.  This is a great way to develop by first defining functional tests and coding underneath as the project progresses.