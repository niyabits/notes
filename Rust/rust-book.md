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

## Concise Control Flow with If Let

