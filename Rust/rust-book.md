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
