---
layout: post
title: "Splitting Mutable Borrows... Splitting Borrowck's Hairs"
description: "Techniques for non-overlapping mutable borrows on container types."
tags: ["Rust"]
---

Please work. Blah blah blah blah. Lorem ipsum or some shit? Please work. Yah blah blah yah. Lorem ipsum or some shit... or some other shitty shit? Who really knows....

As Tanya said,

> Kel that is disgusting. Blah blah blah blah... 
> Lorem ipsum or some shit!
> 
> Delete this.

And so it goes, blah blah blah blah what a mistake software was. 

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

And what a mistake software was. Lorem ipsum or some shit! So in conclusion, who knows what the fuck am I talking about.