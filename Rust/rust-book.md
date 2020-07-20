*Note: This markdown files may not contain the notes of everything about Rust from start because when I made this repo I had already got down some Rust*

## Enum
**Enumeration**
An `enum` defines a set of categories 'something' can fall into.

As an example we have coins of different sizes.
- Penny
- Nickel
- Dime 
- Quarter
and so on...

We can throw in a coin and the coin would be checked one by one 
according to its size.

This is accomplished with `match`.

*Enum VS Struct*  
A  Struct is like - AND  
An Enum   is like - OR  

When a Struct is defined and an instance is created it has to has all the
keys provided in the struture of the struct.

When an Enum is defined, it is generally for `match`ing something, like 
the coin example.

## Matches  
Matches are exhaustive, if we forget to handle a case with match, for e.g. - using some and forgeting a case like none then the Rust compiler will throw an error.

Rust knows that we didn't cover every case, match requires us to exhaust every possibility before moving on.

## The _ placeholder
_ is used in `match`, in situations where we just cannot define every case we use `_` to handle the rest of the cases that are not defined.

For e.g. -
If we have some u8 value, and we are handling the case of 1,3,5 and 7, by doing something special for the rest, we would need to define a behavior like printing "not the number", instead of defining it for all the way upto 255 numbers we can rather say,

`_ => println('not the number')`

## Concise Control Flow with If Let
But what if we just need to handle one single case?

With the match syntax, it is a lot of boilerplate.

We can use `if let` instead.
```rust
if let Some(3) = some_u8_value {
        println!('Three')
    }
```
we can also use `else {}` with if let to handle rest of the cases, 

however, the `if let` thus comes with its own drawbacks.

With `if let` Rust will not perform any exhaustive checking.

# Packages and Crates

*Note*: I have stopped reading about Rust for a while, it is indefinite when I will get back on track with these notes :)
