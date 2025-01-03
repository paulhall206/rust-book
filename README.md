# rust-book
Learning Rust from https://doc.rust-lang.org/book/

# Why learn rust?

Well, that's a good question.  As a long-time C developer, I've spent months hunting memory leaks & corruption in embedded systems.  I still can't abide a kitchen drawer that isn't completely closed: those references must be freed.

I've thumbed K&R for long nights trying to decipher compiler errors and started working with new code by first reformatting it in emacs.

Rust addresses all of those points.  It manages dynamic memory at compile time, has gracious help messages and has made good choices for readability.

Further, I see it being used in embedded systems.  Microsoft's [Surface UEFI](https://techcommunity.microsoft.com/blog/surfaceitpro/surface-uefi-evolution-in-boot-security--device-management-to-build-an-industry-/4159998) now uses Rust as part of Project Mu.  There's another project creating a common trusted processor unit by Microsoft, Nvidia but, sadly, I can't find the link again.  Our friendly mad scientists at [DARPA](https://share.libbyapp.com/title/240436) are embarking on TRAnslating All C TO Rust ([TRACTOR](https://users.rust-lang.org/t/darpa-translating-all-c-to-rust-tractor/115242)).  There must be good things going on.

Finally, learning Rust seems easy. There's a good online book, VS Code has decent support; we'll see how this goes.

# Key Learnings

- Ch 1: Getting Started
    - Install Rust on Windows, Linux or MacOS from [here](https://doc.rust-lang.org/book/ch01-01-installation.html)
    - ```rustup update``` to keep current
    - ```cargo new project_name```, ```cargo build```, ```cargo run``` to create, build and run a project.
    - ```cargo build --release``` for a release build
- Ch 2: Programming a Gussing Game
    - ```cargo doc --open``` awesome documentation for your program and all libraries.  It opens a browser window.  Gotta learn more about this.
    - [https://docs.rs](https://docs.rs) find crate documentation here
    - [https://crates.io/](https://crates.io/) download crates from here
    