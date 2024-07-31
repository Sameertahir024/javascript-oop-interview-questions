# Object-Oriented Programming Interview Questions with JavaScript

## Table of Contents

| No  | Questions                                                                                                    |
| --- | ------------------------------------------------------------------------------------------------------------ |
| 1   | [What is object-oriented Programming?](#answer-1)                                                            |
| 2   | [How does JavaScript support OOP?](#answer-2)      
| 3   | [What is the difference between OOP and SOP?](#answer-3)                              
| 4   | [Why is OOPs so popular?](#answer-4)|
| 5   | [What are the four main principles of OOP?](#answer-5)    
| 6   | [How do you implement Inheritance in JavaScript?](#answer-6)                                               |
| 7   | [How do you implement polymorphism in JavaScript?](#answer-7)                                               |
| 8   | [How do you implement Encapsulation in JavaScript?](#answer-8)                                               |
| 9   | [How do you implement abstraction in JavaScript?](#answer-9)                                               |
| 10  | [How do you create an object in JavaScript?](#answer-10)                                                      |
| 11  | [What is a prototype in JavaScript?](#answer-11)                                                              |
| 12  | [How does prototypal inheritance work in JavaScript?](#answer-12)                                             |
| 13  | [What are closures and how do they relate to OOP?](#answer-13)                                               |
| 14  | [What is the 'this' keyword in JavaScript and how does it work in different contexts?](#answer-14)           |
| 15  | [What are ES6 classes and how do they work?](#answer-15)                                                     |
| 16  | [How do you create private and public methods in JavaScript?](#answer-16)                                    |
| 17  | [What is the difference between function declaration and function expression?](#answer-17)                   |
| 18  | [What is method chaining and how can you implement it?](#answer-18)                                          |
| 19  | [What are getters and setters in JavaScript?](#answer-19)                                                    |
| 20  | [How does the 'new' keyword work in JavaScript?](#answer-20)                                                 |
| 21  | [How do you implement multiple inheritance in JavaScript?](#answer-21)                                       |
| 22  | [What is the purpose of the constructor method in a class?](#answer-22)                                      |
| 23  | [How do you use the 'super' keyword in JavaScript?](#answer-23)                                              |
| 24  | [What is the difference between composition and inheritance?](#answer-24)                                    |
| 25  | [How do you implement a Singleton pattern in JavaScript?](#answer-25)                                        |
| 26  | [What is the Module pattern in JavaScript?](#answer-26)                                                      |
| 27  | [How do you implement the Observer pattern in JavaScript?](#answer-27)                                       |
| 28  | [What is the difference between Object.create() and the new keyword?](#answer-28)                            |
| 29  | [How do you implement method overloading in JavaScript?](#answer-29)                                         |
| 30  | [What is the difference between static and instance methods?](#answer-30)                                    |
| 31  | [How do you use Symbol to create truly private properties?](#answer-31)                                      |
| 32  | [What is the purpose of the 'use strict' directive in JavaScript?](#answer-32)                               |
| 33  | [What is the difference between deep and shallow copying of objects?](#answer-33)                            |
| 34  | [How do you implement method borrowing in JavaScript?](#answer-34)                                           |
| 35  | [What is the difference between call(), apply(), and bind()?](#answer-35)                                    |
| 36  | [What is the difference between Object.assign and Object.create in JavaScript?](#answer-36)                                    |
| 37  | [What is SOLID and how does it apply to JavaScript?](#answer-37)                                             |
| 38  | [What is the difference between abstract classes and interfaces in JavaScript?](#answer-38)                  |
| 39  | [What is the instanceof operator in JavaScript??](#answer-39)                                                |
| 40  | [What is the difference between for...in and for...of loops when dealing with objects?](#answer-40)          |
| 41  | [What are the different types of inheritance?](#answer-41)    
| 42  | [What is the difference between overloading and overriding?](#answer-42)          
| 43  | [What is the difference between **proto** and prototype?](#answer-43)                                        |
| 44  | [What is the difference between instance properties and prototype properties?](#answer-44)                   |
| 45  | [What is the purpose of the instanceof operator?](#answer-45)                                                |
| 46  | [How do you implement method overriding in JavaScript?](#answer-46)                                          |
| 47  | [What is the difference between Object and Map?](#answer-47)                                                 |
| 48  | [What is a Static Method in JavaScript?](#answer-47)                                   |

## 1. <a id="answer-1">What is object-oriented Programming?</a> 
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

[Back to top](#table-of-contents)

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



### <a id="answer-3">Why is OOPs so popular?</a>
The main differences between Object-Oriented Programming (OOP) and Structured Oriented Programming (SOP) are:

Organization:

OOP: Organizes code into objects
SOP: Organizes code into functions and procedures


Data handling:

OOP: Data and methods are bundled together
SOP: Data and functions are separate


Modularity:

OOP: High modularity through objects and classes
SOP: Modularity through functions, but less flexible


Reusability:

OOP: High reusability through inheritance
SOP: Limited reusability, mainly through function calls


Data security:

OOP: Encapsulation provides better data security
SOP: Less control over data access



Example contrasting OOP and SOP approaches:
```javascript
class BankAccount {
  constructor(balance) {
    this.balance = balance;
  }

  deposit(amount) {
    this.balance += amount;
  }

  withdraw(amount) {
    if (amount <= this.balance) {
      this.balance -= amount;
    }
  }
}

const account = new BankAccount(1000);
account.deposit(500);
account.withdraw(200);
```
SOP:
```javascript
let balance = 1000;

function deposit(amount) {
  balance += amount;
}

function withdraw(amount) {
  if (amount <= balance) {
    balance -= amount;
  }
}

deposit(500);
withdraw(200);
```
### <a id="answer-4">Why is OOPs so popular?</a>
OOP (Object-Oriented Programming) is popular for several key reasons:

1.Modularity: Code is organized into reusable objects.

2.Maintainability: Easier to update and modify isolated parts of code.

3.Scalability: Supports building large, complex systems.

4.Code reusability: Objects can be reused across projects.

5.Abstraction: Hides complex implementation details.

5.Real-world modeling: Aligns with how we think about real-world entities.


### <a id="answer-3">What are the four main principles of OOP?</a>

The four main principles of Object-Oriented Programming (OOP) are:

1:Encapsulation: Bundling data and methods that operate on that data within a single unit (class).

2:Inheritance: Ability of a class to derive properties and characteristics from another class.

3:Polymorphism: Ability of objects to take on multiple forms and behave differently based on context.

4:Abstraction: Hiding complex implementation details and showing only essential features of an object.


#### 1. How do you implement Inheritance in JavaScript?
Inheritance in JavaScript can be implemented using the `extends` keyword in classes. This allows a class to inherit properties and methods from another class.

```javascript
class Animal {
  constructor(name) {
    this.name = name;
  }

  speak() {
    console.log(`${this.name} makes a noise.`);
  }
}

class Dog extends Animal {
  constructor(name) {
    super(name);
  }

  speak() {
    console.log(`${this.name} barks.`);
  }
}

const dog = new Dog('Rex');
dog.speak(); // Rex barks.
```


### <a id="answer-4"> How do you implement Polymorphism in JavaScript?</a>
Polymorphism in JavaScript can be implemented through method overriding. Different classes can define methods with the same name, and the appropriate method is called based on the object's type.
```javascript
class Animal {
  speak() {
    console.log('Animal makes a noise.');
  }
}

class Dog extends Animal {
  speak() {
    console.log('Dog barks.');
  }
}

class Cat extends Animal {
  speak() {
    console.log('Cat meows.');
  }
}

const animals = [new Dog(), new Cat()];

animals.forEach(animal => animal.speak());
// Output:
// Dog barks.
// Cat meows.

```


### <a id="answer-4">How do you implement Encapsulation in JavaScript?</a>
Encapsulation in JavaScript can be achieved using closures or ES6 classes with private fields (prefixed with #).
```javascript
class Person {
  #age;

  constructor(name, age) {
    this.name = name;
    this.#age = age;
  }

  getAge() {
    return this.#age;
  }

  setAge(age) {
    if (age > 0) {
      this.#age = age;
    }
  }
}

const person = new Person('John', 30);
console.log(person.getAge()); // 30
person.setAge(31);
console.log(person.getAge()); // 31

```

### <a id="answer-4">How do you implement Abstraction in JavaScript??</a>
Abstraction in JavaScript can be implemented by defining methods in a base class that are overridden by derived classes, hiding the complex details and exposing only the necessary parts.
```javascript
class Employee {
  constructor(name) {
    if (new.target === Employee) {
      throw new TypeError('Cannot construct Employee instances directly');
    }
    this.name = name;
  }

  getDetails() {
    throw new Error('You have to implement the method getDetails!');
  }
}

class Developer extends Employee {
  constructor(name, role) {
    super(name);
    this.role = role;
  }

  getDetails() {
    return `${this.name} is a ${this.role}`;
  }
}

const dev = new Developer('Alice', 'Frontend Developer');
console.log(dev.getDetails()); // Alice is a Frontend Developer

```

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
A static method in JavaScript is a method that belongs to the class itself rather than to instances of the class. Key points about static methods:

Called on the class, not on instances
Cannot access instance-specific data (i.e., can't use 'this' to refer to instance properties)
Often used for utility functions related to the class
```javascript
class MathOperations {
  static add(x, y) {
    return x + y;
  }
  
  static multiply(x, y) {
    return x * y;
  }
}

console.log(MathOperations.add(5, 3));      // Outputs: 8
console.log(MathOperations.multiply(4, 2)); // Outputs: 8

// This would throw an error:
// const math = new MathOperations();
// math.add(1, 2);  // Error: math.add is not a function
```
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
