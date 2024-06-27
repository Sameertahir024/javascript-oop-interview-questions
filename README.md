# Object-Oriented Programming (OOP) Interview Questions with JavaScript

| No. | Question                                                                                   |
|-----|-------------------------------------------------------------------------------------------|
| 1.  | [What is object-oriented Programming?](#answer-1)                                                  |
| 2.  | [Explain inheritance and its types in JavaScript.](#answer-2)                               |
| 3.  | [What is polymorphism in JavaScript? Provide an example.](#answer-3)                        |
| 4.  | [What are classes in JavaScript? Provide syntax and an example.](#answer-4)                  |
| 5.  | [Explain the difference between abstraction and encapsulation.](#answer-5)                  |
| 6.  | [What is method overriding? Provide a JavaScript example.](#answer-6)                       |
| 7.  | [How do you achieve inheritance in ES6 classes?](#answer-7)                                  |
| 8.  | [What is the 'super' keyword used for in JavaScript classes?](#answer-8)                    |
| 9.  | [Explain the concept of interfaces in JavaScript.](#answer-9)                                |
| 10. | [What is composition over inheritance? Provide an example in JavaScript.](#answer-10)        |
| 11. | [How do you implement encapsulation in JavaScript?](#answer-11)                              |
| 12. | [What are static methods in JavaScript classes? Provide an example.](#answer-12)             |
| 13. | [Explain the concept of method overloading in JavaScript.](#answer-13)                       |
| 14. | [What is the prototype chain in JavaScript?](#answer-14)                                     |
| 15. | [How do you create private variables in JavaScript using closures?](#answer-15)              |
| 16. | [Explain the 'this' keyword in JavaScript.](#answer-16)                                       |
| 17. | [What is a constructor in JavaScript? Provide an example.](#answer-17)                       |
| 18. | [What is the difference between shallow copy and deep copy? Provide examples.](#answer-18)   |
| 19. | [How do you implement multiple inheritance in JavaScript?](#answer-19)                       |
| 20. | [What are mixins in JavaScript? Provide an example.](#answer-20)                              |
| ... | ...                                                                                         |
| 100.| ...                                                                                         |

## Answers

### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a coding approach where we organize our code into objects that have data (attributes) and behaviors (methods). In JavaScript, we create objects using object literals or constructor functions. Here’s a simple example:

```javascript
// Example of defining an object using object literal
let person = {
    name: "John",
    age: 30,
    greet: function() {
        console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
    }
};

person.greet(); // Outputs: Hello, my name is John and I am 30 years old.


### <a id="answer-2">Explain inheritance and its types in JavaScript.</a>

Inheritance allows one class (subclass) to inherit the properties and methods of another class (superclass). In JavaScript, inheritance can be achieved through prototype chaining and ES6 classes. Types of inheritance include single inheritance, multiple inheritance, and multilevel inheritance.

### <a id="answer-3">What is polymorphism in JavaScript? Provide an example.</a>

Polymorphism allows methods to behave differently based on the object that calls them. In JavaScript, polymorphism is achieved through method overriding and method overloading.

```javascript
// Example of polymorphism with method overriding
class Animal {
  makeSound() {
    console.log('Animal makes a sound');
  }
}

class Dog extends Animal {
  makeSound() {
    console.log('Dog barks');
  }
}

const dog = new Dog();
dog.makeSound(); // Output: Dog barks
