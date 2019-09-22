---
layout: post
title: "Splitting Mutable Borrows, Splitting Borrowck's Hairs"
description: "Techniques for non-overlapping mutable borrows on container types."
tags: ["Rust"]
---

# Nice.

Please work.

> Tanya
> Said That
> 
> I smell like dookie

```rust
fn nice_function<'a, T: Foo>(foo: T, bar: &'a mut Vec<T>) -> Self {
    let baz: String = "nice".to_string();
    foo.nice(&baz);
    for nice_thing in bar {
        nice_thing += foo.not_nice();
    }
    baz
}
```