# Object-Oriented Programming Interview Questions with JavaScript

## Table of Contents

| # | Questions |
|---|-----------|
| 1 | [What is object-oriented Programming?](#answer-1) |
| 2 | [How does JavaScript support OOP?](#answer-2) |
| 3 | [What are the four main principles of OOP?](#answer-3) |
| 4 | [How do you create an object in JavaScript?](#answer-4) |
| 5 | [What is the difference between object literal notation and constructor function?](#answer-5) |
| 6 | [What is a prototype in JavaScript?](#answer-6) |
| 7 | [How does prototypal inheritance work in JavaScript?](#answer-7) |
| 8 | [What is the difference between classical inheritance and prototypal inheritance?](#answer-8) |
| 9 | [How do you implement encapsulation in JavaScript?](#answer-9) |
| 10 | [What are closures and how do they relate to OOP?](#answer-10) |
| 11 | [How can you achieve abstraction in JavaScript?](#answer-11) |
| 12 | [What is the 'this' keyword in JavaScript and how does it work in different contexts?](#answer-12) |
| 13 | [What are ES6 classes and how do they work?](#answer-13) |
| 14 | [How do you create private and public methods in JavaScript?](#answer-14) |
| 15 | [What is the difference between function declaration and function expression?](#answer-15) |
| 16 | [What is method chaining and how can you implement it?](#answer-16) |
| 17 | [How do you implement polymorphism in JavaScript?](#answer-17) |
| 18 | [What are getters and setters in JavaScript?](#answer-18) |
| 19 | [How does the 'new' keyword work in JavaScript?](#answer-19) |
| 20 | [What is the difference between Object.create() and the new keyword?](#answer-20) |
| 21 | [How do you implement multiple inheritance in JavaScript?](#answer-21) |
| 22 | [What is the purpose of the constructor method in a class?](#answer-22) |
| 23 | [How do you use the 'super' keyword in JavaScript?](#answer-23) |
| 24 | [What is the difference between composition and inheritance?](#answer-24) |
| 25 | [How do you implement a Singleton pattern in JavaScript?](#answer-25) |
| 26 | [What is the Module pattern in JavaScript?](#answer-26) |
| 27 | [How do you implement the Observer pattern in JavaScript?](#answer-27) |
| 28 | [What is the Factory pattern and how is it implemented?](#answer-28) |
| 29 | [How do you implement method overloading in JavaScript?](#answer-29) |
| 30 | [What is the difference between static and instance methods?](#answer-30) |
| 31 | [How do you use Symbol to create truly private properties?](#answer-31) |
| 32 | [What are WeakMap and WeakSet, and how are they used in OOP?](#answer-32) |
| 33 | [How do you implement mixins in JavaScript?](#answer-33) |
| 34 | [What is the difference between Object.seal() and Object.freeze()](#answer-34) |
| 35 | [How do you use Object.defineProperty()?](#answer-35) |
| 36 | [What is the purpose of the 'use strict' directive in JavaScript?](#answer-36) |
| 37 | [How do you implement a decorator pattern in JavaScript?](#answer-37) |
| 38 | [What is the difference between deep and shallow copying of objects?](#answer-38) |
| 39 | [How do you implement method borrowing in JavaScript?](#answer-39) |
| 40 | [What is the difference between call(), apply(), and bind()?](#answer-40) |
| 41 | [How do you implement a chain of responsibility pattern?](#answer-41) |
| 42 | [What is SOLID and how does it apply to JavaScript?](#answer-42) |
| 43 | [How do you implement the Strategy pattern in JavaScript?](#answer-43) |
| 44 | [What is the difference between abstract classes and interfaces in JavaScript?](#answer-44) |
| 45 | [How do you implement namespacing in JavaScript?](#answer-45) |
| 46 | [What is the revealing module pattern?](#answer-46) |
| 47 | [How do you use Object.create() for inheritance?](#answer-47) |
| 48 | [What is the difference between for...in and for...of loops when dealing with objects?](#answer-48) |
| 49 | [How do you implement a Proxy object in JavaScript?](#answer-49) |
| 50 | [What is the purpose of the Object.is() method?](#answer-50) |
| 51 | [How do you use Object.assign() for object composition?](#answer-51) |
| 52 | [What is the difference between __proto__ and prototype?](#answer-52) |
| 53 | [How do you implement a memoization pattern in JavaScript?](#answer-53) |
| 54 | [What is the difference between instance properties and prototype properties?](#answer-54) |
| 55 | [How do you implement the Command pattern in JavaScript?](#answer-55) |
| 56 | [What is the purpose of the instanceof operator?](#answer-56) |
| 57 | [How do you implement method overriding in JavaScript?](#answer-57) |
| 58 | [What is the difference between Object.preventExtensions(), Object.seal(), and Object.freeze()?](#answer-58) |
| 59 | [How do you implement the Mediator pattern in JavaScript?](#answer-59) |
| 60 | [What is the purpose of the Object.keys() method?](#answer-60) |
| 61 | [How do you implement a fluent interface in JavaScript?](#answer-61) |
| 62 | [What is the difference between function constructors and factory functions?](#answer-62) |
| 63 | [How do you implement the Adapter pattern in JavaScript?](#answer-63) |
| 64 | [What is the purpose of the Object.values() method?](#answer-64) |
| 65 | [How do you implement the Builder pattern in JavaScript?](#answer-65) |
| 66 | [What is the difference between Object.entries() and Object.fromEntries()?](#answer-66) |
| 67 | [How do you implement the State pattern in JavaScript?](#answer-67) |
| 68 | [What is the purpose of the Object.getOwnPropertyDescriptor() method?](#answer-68) |
| 69 | [How do you implement the Facade pattern in JavaScript?](#answer-69) |
| 70 | [What is the difference between hasOwnProperty() and in operator?](#answer-70) |
| 71 | [How do you implement the Iterator pattern in JavaScript?](#answer-71) |
| 72 | [What is the purpose of the Object.getPrototypeOf() method?](#answer-72) |
| 73 | [How do you implement the Composite pattern in JavaScript?](#answer-73) |
| 74 | [What is the difference between Object.keys() and Object.getOwnPropertyNames()?](#answer-74) |
| 75 | [How do you implement the Flyweight pattern in JavaScript?](#answer-75) |
| 76 | [What is the purpose of the Object.setPrototypeOf() method?](#answer-76) |
| 77 | [How do you implement the Bridge pattern in JavaScript?](#answer-77) |
| 78 | [What is the difference between enumerable and non-enumerable properties?](#answer-78) |
| 79 | [How do you implement the Visitor pattern in JavaScript?](#answer-79) |
| 80 | [What is the purpose of the Reflect API in JavaScript?](#answer-80) |
| 81 | [How do you implement the Template Method pattern in JavaScript?](#answer-81) |
| 82 | [What is the difference between Object and Map?](#answer-82) |
| 83 | [How do you implement the Memento pattern in JavaScript?](#answer-83) |
| 84 | [What is the purpose of the Symbol.species property?](#answer-84) |
| 85 | [How do you implement the Interpreter pattern in JavaScript?](#answer-85) |
| 86 | [What is the difference between imperative and declarative programming in OOP context?](#answer-86) |
| 87 | [How do you implement the Prototype pattern in JavaScript?](#answer-87) |
| 88 | [What is the purpose of the new.target metaproperty?](#answer-88) |
| 89 | [How do you implement the Null Object pattern in JavaScript?](#answer-89) |
| 90 | [What is the difference between aggregation and composition in OOP?](#answer-90) |
| 91 | [How do you implement the Lazy Loading pattern in JavaScript?](#answer-91) |
| 92 | [What is the purpose of the Object.getOwnPropertySymbols() method?](#answer-92) |
| 93 | [How do you implement the Dependency Injection pattern in JavaScript?](#answer-93) |
| 94 | [What is the difference between tight coupling and loose coupling?](#answer-94) |
| 95 | [How do you implement the Unit of Work pattern in JavaScript?](#answer-95) |
| 96 | [What is the purpose of the Object.isExtensible() method?](#answer-96) |
| 97 | [How do you implement the Repository pattern in JavaScript?](#answer-97) |
| 98 | [What is the difference between method chaining and method cascading?](#answer-98) |
| 99 | [How do you implement the Specification pattern in JavaScript?](#answer-99) |
| 100 | [What is the purpose of the Object.isFrozen() method?](#answer-100) |
