---
title: "Differences between Types and Interfaces in TypeScript"
seoTitle: "Differences Between Types and interfaces in TypeScript."
seoDescription: "This is a short article where I wrote to show the differences between Types and Interfaces."
datePublished: Wed May 17 2023 00:41:50 GMT+0000 (Coordinated Universal Time)
cuid: clhqz9st2000409mj86rx0sm6
slug: differences-between-types-and-interfaces-in-typescript
tags: typescript

---

TypeScript is a statically typed programming language that extends JavaScript by adding types. It offers two ways of defining types: types and interfaces. While both types and interfaces are used for defining custom types, they have some differences in how they work and what they offer.

## Interfaces

An interface in TypeScript is a way of defining a contract that an object must adhere to. It is a set of rules that an object must follow to be considered of a particular type. Interfaces can define properties, methods, and index signatures that an object must have. Here is an example of an interface:

```typescript
interface Person {

  name: string;

  age: number;

  sayHello(): void;

}
```

This interface defines a type called `Person`, which has three properties: `name` of type `string`, `age` of type `number`, and `sayHello` method that returns `void`. To create an object that adheres to this interface, we must define all three properties and implement the `sayHello` method:

```typescript
const person: Person = {

  name: 'John',

  age: 30,

  sayHello() {console.log()}, };
```

Interfaces can also extend other interfaces, allowing us to build complex types from smaller ones:

```typescript
interface Employee extends Person {

position: string;

}
```

This interface extends the `Person` interface and adds a `position` property of type `string`. Now, any object that adheres to the `Employee` interface must have all the properties of `Person` as well as the `position` property.

## Types

A type in TypeScript is a way of defining a custom type that can be used throughout the codebase. It is similar to an interface, but it can define more than just objects. Types can define union types, intersection types, tuple types, and more. Here is an example of a type:

```typescript
type Person = {
```

This type defines the same `Person` type as the interface above. However, it uses the `type` keyword instead of `interface`. To create an object that adheres to this type, we use the same syntax as with interfaces:

```typescript
const person: Person = {

name: 'John',

age: 30,

sayHello() {

console.log(`Hello, my name is ${this.name}`);

},

};
```

Like interfaces, types can also be extended to create more complex types:

```typescript
type Employee = Person & {

position: string;

};
```

This type defines an `Employee` type that extends the `Person` type and adds a `position` property of type `string`. Now, any object that adheres to the `Employee` type must have all the properties of `Person` as well as the `position` property.

## Differences

While interfaces and types are similar in many ways, they have some differences that make them useful in different situations:

* Interfaces can be implemented by classes, while types cannot. This makes interfaces more suitable for defining APIs and contracts that must be implemented by multiple classes.
    
* Types can define more complex types than interfaces, such as union types, intersection types, and mapped types. This makes types more suitable for defining complex data structures and types that are used throughout the codebase.
    
* Interfaces can be extended by other interfaces, while types can be intersected with other types. This makes interfaces more suitable for building complex types from smaller ones.
    

In summary, types and interfaces in TypeScript are two ways of defining custom types. While they are similar in many ways, they have some differences that make them useful in different situations. Interfaces are more suitable for defining APIs and contracts, while types are more suitable for defining complex data structures and types that are used throughout the codebase.