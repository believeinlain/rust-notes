# Rust Notes
A collection of notes and resources about Rust for learning Rust development.  

## Projects
[rust-hello-world](https://github.com/believeinlain/rust-hello-world.git)  
An introductory project to familiarize myself with Rust development. Has some useful notes and resources on Windows development in Rust and project organization.

## Functional Programming in Rust
I like functional programming, and I think building a functional game engine in Rust would be a fun exercise. [This article](https://kerkour.com/rust-functional-programming) goes into some of Rust's features that make it amenable to functional programming.

In short:  
- Statements in Rust typically evaluate to values, so return statements are optional.
- Variables in Rust are immutable by default.
- Functions are first-class in Rust and can be manipulated and transformed just like other data types.
- Rust collections have built-in functions such as `for_each`, `reduce`, `fold`, `map`, etc.
- Rust has a data-parallelism library [rayon](https://github.com/rayon-rs/rayon) to support multi-threading without worrying about synchronization.

## Rust Game Engine
To design a functional game engine, I need to start with safe, cross-platform Rust packages. OpenGL wrappers seem to be a good place to start.  

[glutin](https://github.com/rust-windowing/glutin) provides low-level Rust bindings for creating an OpenGL context and handling events.  
[glium](https://docs.rs/glium/latest/glium/) is based on glutin, but provides a complete OpenGL3+ wrapper, and claims to be safe.  
[wgpu](https://docs.rs/wgpu/latest/wgpu/) is a cross-platform library based on WebGPU rather than OpenGL. I should compare WebGPU and OpenGL and see which one would be better to learn, although I've kind of always wanted to learn OpenGL and I'm already familiar with a lot how it works.  

[Here](http://nercury.github.io/rust/opengl/tutorial/2018/02/08/opengl-in-rust-from-scratch-00-setup.html) is an article covering how to wrap OpenGL from Rust - I should read through it even if I use existing wrappers so that I understand what's going on.  

[amethyst](https://github.com/amethyst/amethyst) is an abandoned game engine that encorporates the Entity Component System (ECS) model and claims to be data-oriented, so there may be something good to glean from its design. The devs recommend [this book](https://pragprog.com/titles/hwrust/hands-on-rust/). [This artice](https://amethyst.rs/posts/amethyst--starting-fresh) has some other good resources as well.  
[bevy](https://bevyengine.org) is another data-driven game engine in Rust that seems to be actively maintained.  

## Quantum Computing
Maybe it would be fun to rebuild my quantum computer emulator in Rust. Cool resources: https://arewequantumyet.github.io  

## Hands-on Rust
Just bought the book [Hands-on Rust Effective Learning through 2D Game Development and Play by Herbert Wolverson](https://pragprog.com/titles/hwrust/hands-on-rust/).

Working through the examples [here](https://github.com/believeinlain/hands-on-rust.git).