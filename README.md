# Object-Oriented Programming Interview Questions with JavaScript

## Table of Contents

| No  | Questions                                                                                                    |
| --- | ------------------------------------------------------------------------------------------------------------ |
| 1   | [What is object-oriented Programming?](#answer-1)                                                            |
| 2   | [How does JavaScript support OOP?](#answer-2)                                                                |
| 3   | [What are the four main principles of OOP?](#answer-3)                                                       |
| 4   | [How do you create an object in JavaScript?](#answer-4)                                                      |
| 5   | [What is the difference between object literal notation and constructor function?](#answer-5)                |
| 6   | [What is a prototype in JavaScript?](#answer-6)                                                              |
| 7   | [How does prototypal inheritance work in JavaScript?](#answer-7)                                             |
| 8   | [What is the difference between classical inheritance and prototypal inheritance?](#answer-8)                |
| 9   | [How do you implement encapsulation in JavaScript?](#answer-9)                                               |
| 10  | [What are closures and how do they relate to OOP?](#answer-10)                                               |
| 11  | [How can you achieve abstraction in JavaScript?](#answer-11)                                                 |
| 12  | [What is the 'this' keyword in JavaScript and how does it work in different contexts?](#answer-12)           |
| 13  | [What are ES6 classes and how do they work?](#answer-13)                                                     |
| 14  | [How do you create private and public methods in JavaScript?](#answer-14)                                    |
| 15  | [What is the difference between function declaration and function expression?](#answer-15)                   |
| 16  | [What is method chaining and how can you implement it?](#answer-16)                                          |
| 17  | [How do you implement polymorphism in JavaScript?](#answer-17)                                               |
| 18  | [What are getters and setters in JavaScript?](#answer-18)                                                    |
| 19  | [How does the 'new' keyword work in JavaScript?](#answer-19)                                                 |
| 20  | [What is the difference between Object.create() and the new keyword?](#answer-20)                            |
| 21  | [How do you implement multiple inheritance in JavaScript?](#answer-21)                                       |
| 22  | [What is the purpose of the constructor method in a class?](#answer-22)                                      |
| 23  | [How do you use the 'super' keyword in JavaScript?](#answer-23)                                              |
| 24  | [What is the difference between composition and inheritance?](#answer-24)                                    |
| 25  | [How do you implement a Singleton pattern in JavaScript?](#answer-25)                                        |
| 26  | [What is the Module pattern in JavaScript?](#answer-26)                                                      |
| 27  | [How do you implement the Observer pattern in JavaScript?](#answer-27)                                       |
| 28  | [What is the Factory pattern and how is it implemented?](#answer-28)                                         |
| 29  | [How do you implement method overloading in JavaScript?](#answer-29)                                         |
| 30  | [What is the difference between static and instance methods?](#answer-30)                                    |
| 31  | [How do you use Symbol to create truly private properties?](#answer-31)                                      |
| 32  | [What is a closure in JavaScript??](#answer-32)                                      |
| 33  | [How do you implement mixins in JavaScript?](#answer-33)                                                     |
| 34  | [What is the difference between Object.seal() and Object.freeze()](#answer-34)                               |
| 35  | [How do you use Object.defineProperty()?](#answer-35)                                                        |
| 36  | [What is the purpose of the 'use strict' directive in JavaScript?](#answer-36)                               |
| 38  | [What is the difference between deep and shallow copying of objects?](#answer-38)                            |
| 39  | [How do you implement method borrowing in JavaScript?](#answer-39)                                           |
| 40  | [What is the difference between call(), apply(), and bind()?](#answer-40)                                    |
| 41  | [What is the difference between Object.assign and Object.create in JavaScript?](#answer-41)                                    |
| 42  | [What is SOLID and how does it apply to JavaScript?](#answer-42)                                             |
| 44  | [What is the difference between abstract classes and interfaces in JavaScript?](#answer-44)                  |
| 45  | [How do you implement namespacing in JavaScript?](#answer-45)                                                |
| 46  | [What is the instanceof operator in JavaScript??](#answer-46)                                                |
| 47  | [How do you use Object.create() for inheritance?](#answer-47)                                                |
| 48  | [What is the difference between for...in and for...of loops when dealing with objects?](#answer-48)          |
| 49  | [Why is OOPs so popular?](#answer-49)          
|     | [What is the difference between overloading and overriding?](#answer-)          
| 52  | [What is the difference between **proto** and prototype?](#answer-52)                                        |
| 54  | [What is the difference between instance properties and prototype properties?](#answer-54)                   |
| 55  | [How do you implement the Command pattern in JavaScript?](#answer-55)                                        |
| 56  | [What is the purpose of the instanceof operator?](#answer-56)                                                |
| 57  | [How do you implement method overriding in JavaScript?](#answer-57)                                          |
| 60  | [What is the purpose of the Object.keys() method?](#answer-60)                                               |
| 61  | [How do you implement a fluent interface in JavaScript?](#answer-61)                                         |
| 62  | [What is the difference between function constructors and factory functions?](#answer-62)                    |
| 70  | [What is the difference between hasOwnProperty() and in operator?](#answer-70)                               |
| 71  | [How do you implement the Iterator pattern in JavaScript?](#answer-71)                                       |
| 74  | [What is the difference between Object.keys() and Object.getOwnPropertyNames()?](#answer-74)                 |
| 82  | [What is the difference between Object and Map?](#answer-82)                                                 |
| 85  | [How do you implement the Interpreter pattern in JavaScript?](#answer-85)                                    |
| 87  | [How do you implement the Prototype pattern in JavaScript?](#answer-87)                                      |
| 89  | [How do you implement the Null Object pattern in JavaScript?](#answer-89)                                    |
| 90  | [What is the difference between aggregation and composition in OOP?](#answer-90)                             |
| 91  | [How do you implement the Lazy Loading pattern in JavaScript?](#answer-91)                                   |
| 92  | [What is a Static Method in JavaScript?](#answer-92)                                   |
| 93  | [How do you implement the Dependency Injection pattern in JavaScript?](#answer-93)                           |
| 94  | [What is the difference between tight coupling and loose coupling?](#answer-94)                              |
| 95  | [How do you implement the Unit of Work pattern in JavaScript?](#answer-95)                                   |                                  
| 97  | [How do you implement the Repository pattern in JavaScript?](#answer-97)                                     |
| 98  | [What is the difference between method chaining and method cascading?](#answer-98)                           |
| 99  | [How do you implement the Specification pattern in JavaScript?](#answer-99)                                  |
|

## Answers

### <a id="answer-1">What is object-oriented Programming?</a>
Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)

### <a id="answer-2">How does JavaScript support OOP??</a>

JavaScript supports Object-Oriented Programming (OOP) through:

1:Objects
2:Classes (ES6+)
3:Prototypes
4:Inheritance

Example using a class:
```javascript
class Car {
  constructor(brand) {
    this.brand = brand;
  }
  
  drive() {
    console.log(`Driving a ${this.brand}`);
  }
}

const myCar = new Car("Toyota");
myCar.drive(); // Outputs: Driving a Toyota

```

[↑ Go back](#question-2)


### <a id="answer-3">What are the four main principles of OOP?</a>


### <a id="answer-4">How do you create an object in JavaScript?</a>
In JavaScript, there are several ways to create an object. Here are a few common methods:

## 1. Using Object Literal Syntax
```javascript
const person = {
    name: 'John',
    age: 30,
    greet: function() {
        console.log('Hello, ' + this.name);
    }
};

person.greet(); // Output: Hello, John
```
## 2. Using the new Object() Syntax
```javascript
const person = new Object();
person.name = 'John';
person.age = 30;
person.greet = function() {
    console.log('Hello, ' + this.name);
};

person.greet(); // Output: Hello, John

```
## 3. Using a Constructor Function
```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
    this.greet = function() {
        console.log('Hello, ' + this.name);
    };
}

const person = new Person('John', 30);
person.greet(); // Output: Hello, John

```
## 4. Using ES6 Classes
```javascript
class Person {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }

    greet() {
        console.log('Hello, ' + this.name);
    }
}

const person = new Person('John', 30);
person.greet(); // Output: Hello, John


```

### <a id="answer-5">What is the difference between object literal notation and constructor function?</a>
## Object Literal Notation
Object literal notation is a simple and concise way to create objects in JavaScript. It is best suited for creating single objects or objects that do not require a blueprint.
```javascript
const person = {
    name: 'John',
    age: 30,
    greet: function() {
        console.log('Hello, ' + this.name);
    }
};

person.greet(); // Output: Hello, John
```
## Constructor Function
Definition: A constructor function is a template for creating multiple objects with the same properties and methods. It uses the function keyword and can be instantiated using the new keyword.
```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
    this.greet = function() {
        console.log('Hello, ' + this.name);
    };
}

const person1 = new Person('John', 30);

```


### <a id="answer-6">What is a prototype in JavaScript?</a>
In JavaScript, every object has a prototype. A prototype is an object from which other objects inherit properties and methods. Prototypes allow you to add properties and methods to objects after they are created, which enables inheritance and the reuse of code.
```javascript
// Constructor function
function Person(name, age) {
    this.name = name;
    this.age = age;
}

// Adding a method to the prototype
Person.prototype.greet = function() {
    console.log('Hello, ' + this.name);
};

// Creating objects
const person1 = new Person('John', 30);
const person2 = new Person('Jane', 25);

person1.greet(); // Output: Hello, John
person2.greet(); // Output: Hello, Jane

```

### <a id="answer-7">How does prototypal inheritance work in JavaScript?</a>
pending................................
### <a id="answer-8">What is the difference between classical inheritance and prototypal inheritance?</a>
pending........................
### <a id="answer-9">What is object-oriented Programming?</a>
### <a id="answer-10">What is object-oriented Programming?</a>
### <a id="answer-11">What is object-oriented Programming?</a>
### <a id="answer-12">What is object-oriented Programming?</a>
### <a id="answer-13">What is object-oriented Programming?</a>
### <a id="answer-14">What is object-oriented Programming?</a>
### <a id="answer-15">What is object-oriented Programming?</a>
### <a id="answer-16">What is object-oriented Programming?</a>
### <a id="answer-17">What is object-oriented Programming?</a>
### <a id="answer-18">What are getters and setters in JavaScript?</a>
In JavaScript, getters and setters are special methods that allow you to define the behavior of accessing and setting values on an object's properties.

Getter: A getter is a method that gets the value of a specific property. It is defined using the get keyword followed by a function. When you access the property, the getter function is executed, and its return value is used as the property value.
```javascript
const obj = {
    get fullName() {
        return `${this.firstName} ${this.lastName}`;
    },
    firstName: 'John',
    lastName: 'Doe'
};

console.log(obj.fullName); // Outputs: "John Doe"

```
Setter: A setter is a method that sets the value of a specific property. It is defined using the set keyword followed by a function that takes a parameter representing the new value. When you assign a value to the property, the setter function is called with the assigned value.
```javascript
const obj = {
    firstName: 'John',
    lastName: 'Doe',
    set fullName(value) {
        const [first, last] = value.split(' ');
        this.firstName = first;
        this.lastName = last;
    }
};

obj.fullName = 'Jane Smith';
console.log(obj.firstName); // Outputs: "Jane"
console.log(obj.lastName); // Outputs: "Smith"


```

### <a id="answer-19">How does the 'new' keyword work in JavaScript?</a>
In JavaScript, the new keyword is used to create an instance of a user-defined object type (often called a constructor function) or a built-in object type that has a constructor function. Here's how it works:

Creating an Instance: When you use new with a constructor function, it creates a new object instance. This new instance inherits properties and methods defined on the constructor's prototype.
```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
}

const john = new Person('John', 30);
```


### <a id="answer-20">What is the difference between Object.create() and the new keyword?</a>
The Object.create() method and the new keyword in JavaScript serve different purposes for object creation and inheritance:

## Object.create():

Purpose: Creates a new object with the specified prototype object and optionally defines its properties.
Syntax: Object.create(proto [, propertiesObject])

```javascript
const protoObj = {
    greet() {
        console.log(`Hello, ${this.name}!`);
    }
};

const obj = Object.create(protoObj, {
    name: { value: 'John' }
});

obj.greet(); // Outputs: "Hello, John!"

```
## new Keyword:

Purpose: Creates an instance of a constructor function, which typically defines properties and methods for the objects it creates.
```javascript
function Person(name) {
    this.name = name;
}

const john = new Person('John');

```

### <a id="answer-21">How do you implement multiple inheritance in JavaScript?</a>

pending...................
### <a id="answer-22">What is the purpose of the constructor method in a class?</a>
Purpose of the Constructor Method in a Class:
1: Initialization: Sets up initial values for object properties.

2: State Setup: Establishes the initial state of the object.

3: Binding: Binds methods to the instance.
3: Inheritance: Calls super() to initialize properties from a parent class.
```javascript
class Person {
    // Constructor method
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }
}

const john = new Person('John', 30);
console.log(john.name); // Outputs: "John"
console.log(john.age); // Outputs: 30

```
### <a id="answer-23">How do you use the 'super' keyword in JavaScript?</a>
Purpose of the super Keyword in JavaScript:
## Constructor Calls:
Allows calling the constructor of a parent class from within a subclass constructor to initialize inherited properties.
## Method Calls:
Facilitates invoking methods from the parent class within subclass methods to extend or override their behavior.
```javascript
// Parent class
class Animal {
    constructor(name) {
        this.name = name;
    }

    makeSound() {
        console.log("Animal makes a sound");
    }
}

// Subclass extending Animal
class Dog extends Animal {
    constructor(name, breed) {
        super(name); // Calling parent constructor
        this.breed = breed;
    }

    makeSound() {
        super.makeSound(); // Calling parent method
        console.log("Woof!");
    }
}

// Creating an instance of Dog
const myDog = new Dog('Buddy', 'Labrador');

// Using the subclass methods and inherited properties
console.log(myDog.name); // Outputs: "Buddy"
myDog.makeSound(); // Outputs:
// "Animal makes a sound"
// "Woof!"

```
### <a id="answer-24">What is object-oriented Programming?</a>
pending.....................

### <a id="answer-25">How do you implement a Singleton pattern in JavaScript?</a>
pending......................

### <a id="answer-26">What is the Module pattern in JavaScript?</a>
The Module pattern in JavaScript is a design pattern used to create encapsulated and reusable code. It provides a way to create private and public methods and variables, helping to shield particular parts from the global scope.
Key features:

1:Encapsulation

2:Privacy

3:Organization

Example:
```javascript
const Calculator = (function() {
  // Private variable
  let result = 0;
  
  // Public methods
  return {
    add: function(x) {
      result += x;
    },
    subtract: function(x) {
      result -= x;
    },
    getResult: function() {
      return result;
    }
  };
})();

Calculator.add(5);
Calculator.subtract(2);
console.log(Calculator.getResult()); // Outputs: 3
console.log(Calculator.result); // Outputs: undefined
```
### <a id="answer-27">How do you implement the Observer pattern in JavaScript?</a>
pending....................

### <a id="answer-28">What is object-oriented Programming?</a>
### <a id="answer-29">What is object-oriented Programming?</a>
### <a id="answer-30">What is object-oriented Programming?</a>
### <a id="answer-31">What is object-oriented Programming?</a>
### <a id="answer-32">What is object-oriented Programming?</a>
### <a id="answer-33">What is object-oriented Programming?</a>
### <a id="answer-34">What is object-oriented Programming?</a>
### <a id="answer-35">What is object-oriented Programming?</a>
### <a id="answer-36">What is the purpose of the 'use strict' directive in JavaScript?</a>

The 'use strict' directive in JavaScript enables strict mode, which enforces stricter parsing and error handling rules. Its main purposes are:

Catch coding mistakes
Prevent unsafe actions
Disable confusing or poorly thought-out features
```javascript
'use strict';

// Without strict mode, this would create a global variable
x = 3.14;  // Throws ReferenceError

function example() {
  'use strict';
  
  // Prevents accidental global variable creation
  y = 10;  // Throws ReferenceError
  
  // Prevents using reserved keywords as variable names
  let interface = 'hello';  // Throws SyntaxError
  
  // Makes eval() safer
  eval('var z = 42');
  console.log(z);  // Throws ReferenceError
}

example();
```
### <a id="answer-37">What is object-oriented Programming?</a>
### <a id="answer-38">What is object-oriented Programming?</a>
### <a id="answer-39">What is object-oriented Programming?</a>
### <a id="answer-40">What is the difference between call(), apply(), and bind()?</a>

The main differences between call(), apply(), and bind() are:

call(): Invokes a function with a specified 'this' context and arguments passed individually.
apply(): Similar to call(), but arguments are passed as an array.
bind(): Returns a new function with a fixed 'this' context, without invoking it immediately.

Example:
```javascript
const person = { name: 'John' };

function greet(greeting, punctuation) {
  console.log(`${greeting}, ${this.name}${punctuation}`);
}

// call()
greet.call(person, 'Hello', '!');  // Output: Hello, John!

// apply()
greet.apply(person, ['Hi', '?']);  // Output: Hi, John?

// bind()
const boundGreet = greet.bind(person);
boundGreet('Hey', '.');  // Output: Hey, John.
```
### <a id="answer-41">What is object-oriented Programming?</a>
### <a id="answer-42">What is object-oriented Programming?</a>
### <a id="answer-43">What is object-oriented Programming?</a>
### <a id="answer-44">What is object-oriented Programming?</a>
### <a id="answer-45">What is object-oriented Programming?</a>
### <a id="answer-46">What is object-oriented Programming?</a>
### <a id="answer-47">What is object-oriented Programming?</a>
### <a id="answer-48">What is object-oriented Programming?</a>
### <a id="answer-49">What is object-oriented Programming?</a>
### <a id="answer-50">What is object-oriented Programming?</a>
### <a id="answer-51">What is object-oriented Programming?</a>
### <a id="answer-52">What is the difference between **proto** and prototype?</a>
The key differences between proto and prototype are:

proto:

Property of object instances
Points to the prototype of the constructor function
Part of the object's prototype chain


prototype:

Property of constructor functions
Contains shared properties/methods for instances
Used to implement inheritance
```javascript
function Dog(name) {
  this.name = name;
}

Dog.prototype.bark = function() {
  console.log(this.name + ' says woof!');
};

const dog1 = new Dog('Buddy');

console.log(dog1.__proto__ === Dog.prototype);  // true
console.log(Dog.prototype.isPrototypeOf(dog1)); // true

dog1.bark();  // Outputs: Buddy says woof!
```
### <a id="answer-53">What is object-oriented Programming?</a>
### <a id="answer-54">What is object-oriented Programming?</a>
### <a id="answer-55">What is object-oriented Programming?</a>
### <a id="answer-56">What is object-oriented Programming?</a>
### <a id="answer-57">What is object-oriented Programming?</a>
### <a id="answer-58">What is object-oriented Programming?</a>
### <a id="answer-59">What is object-oriented Programming?</a>
### <a id="answer-60">What is object-oriented Programming?</a>
### <a id="answer-61">What is object-oriented Programming?</a>
### <a id="answer-62">What is object-oriented Programming?</a>
### <a id="answer-63">What is object-oriented Programming?</a>
### <a id="answer-64">What is object-oriented Programming?</a>
### <a id="answer-65">What is object-oriented Programming?</a>
### <a id="answer-66">What is object-oriented Programming?</a>
### <a id="answer-67">What is object-oriented Programming?</a>
### <a id="answer-68">What is object-oriented Programming?</a>
### <a id="answer-69">What is object-oriented Programming?</a>
### <a id="answer-70">What is object-oriented Programming?</a>
### <a id="answer-71">What is object-oriented Programming?</a>
### <a id="answer-71">What is object-oriented Programming?</a>
### <a id="answer-72">What is object-oriented Programming?</a>
### <a id="answer-73">What is object-oriented Programming?</a>
### <a id="answer-74">What is object-oriented Programming?</a>
### <a id="answer-75">What is object-oriented Programming?</a>
### <a id="answer-76">What is object-oriented Programming?</a>
### <a id="answer-77">What is object-oriented Programming?</a>
### <a id="answer-78">What is object-oriented Programming?</a>
### <a id="answer-79">What is object-oriented Programming?</a>
### <a id="answer-80">What is object-oriented Programming?</a>
### <a id="answer-81>What is object-oriented Programming?</a>
### <a id="answer-82">What is object-oriented Programming?</a>
### <a id="answer-83">What is object-oriented Programming?</a>
### <a id="answer-84">What is object-oriented Programming?</a>
### <a id="answer-85">What is object-oriented Programming?</a>
### <a id="answer-86">What is object-oriented Programming?</a>
### <a id="answer-87">What is object-oriented Programming?</a>
### <a id="answer-88">What is object-oriented Programming?</a>
### <a id="answer-89">What is object-oriented Programming?</a>
### <a id="answer-90">What is object-oriented Programming?</a>
### <a id="answer-91">What is object-oriented Programming?</a>
### <a id="answer-92">What is object-oriented Programming?</a>
### <a id="answer-93">What is object-oriented Programming?</a>
### <a id="answer-94">What is object-oriented Programming?</a>
### <a id="answer-95">What is object-oriented Programming?</a>
### <a id="answer-96">What is object-oriented Programming?</a>
### <a id="answer-97">What is object-oriented Programming?</a>
### <a id="answer-98">What is object-oriented Programming?</a>
### <a id="answer-99">What is object-oriented Programming?</a>
### <a id="answer-100">What is object-oriented Programming?</a>




### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)
### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)
### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)
### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)
### <a id="answer-1">What is object-oriented Programming?</a>

Object-oriented programming (OOP) is a way to structure code by creating objects, which are instances of classes. A class defines the properties and methods that its objects will have, making the code more organized and reusable.

```javascript
// Define a class
class Car {
  constructor(make, model) {
    this.make = make;
    this.model = model;
  }

  // Method to display car details
  displayInfo() {
    return `${this.make} ${this.model}`;
  }
}

// Create an object
const myCar = new Car("Toyota", "Corolla");
console.log(myCar.displayInfo()); // Output: Toyota Corolla
```

[↑ Go back](#question-1)
JavaScript supports Object-Oriented Programming (OOP) through:

Objects
Classes (ES6+)
Prototypes
Inheritance

Example using a class:
