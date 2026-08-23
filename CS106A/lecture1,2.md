The lecture introduces Karel(Carol) the Robot and carry it throughout the session to teach basic coding logic, loops, and control flows..

#### What is Karel the Robot again?

Its a coding game that offers a series of levels, by clearing which, the users learn a new programming concept.
For more info check out:
https://compedu.stanford.edu/karel-reader/docs/python/en/chapter1.html

### Program Vs Algorithm:

Statements that are valid according to the syntactically rules of the language.

Algorithm is the recipe for doing something

### When writing the program

1. We define a run method.
2. The run method helps executing the program by **encapsultaing** everything at one place.
3. We can then list all the intructions inside.

## How does Karel works?

1. It comes with predefined set of commands that can be executed in JAVA, Python etc (depends on what Karol version you consume)
2. It is encapsulated inside a class in Java to ensure all its properties are unified and accessible from anywhere in the code.
3. To run it, in Java, we do:

```
import standford.karel.*;

public class OurKarelProgram extends Karel{

    public void run(){
        move();
        pickBeeper();
        ...
    }
}
```

### What does this code mean?

- Import helps us add a reference to Karel methods(commands) and properties
- Notice, we also define a class to encapsulate our code.
- Extends (**Inherits**) ensure we get access to Karel commands like move() etc 
- run() helps us keep all the commands at one place to ensure easy execution.

Finally hit the run!

Other Questions?

- The methods also contains set of instructions
- They are case Sensitive :)

### Create you own methods

```
public void turnAround(){
    turnLeft();
    turnRight();
}
```

### If we want repitiion?

```
For loops!

for (int i=0; i<3 ; i++){
    turnLeft();
}
```

But if you only have a condition? use while
```
while(frontIsClear()){
move();
}
```

### You have more conditions?

Then you have If

```
if(beeperPresent()){
pickBeeper();
}
else{
putBeeper();
}
```

and nest them

> Code should be General that fits any particular scenario.



## Common Errors

**OBUB** - **O**ff **B**y **O**ne **B**ug
This mean that one more thing that your code should have done, but instead it encountered a bug. 


### Comments
To make program readable. 
Good practice is to put comment before each method.

## Decomposition
### Top Down Design
### Bottom Up Design 

Based on the lecture, a smart statergy isto write code with intuition using top down. First define the principle tasks in the main methods, then for each of them write secondary and so on. 

> Every method should solve One and Only one problem

> methods shouldn't be longer than 15 lines (honestly 30-40 is fine too)

> Methods should have good names

> Comments are must



## History of Computing Languages
4000 years ago abacus was the first computing device.
1800s - **Charles Babbage** devised different engine that became analytical engine.

First Programmer was **Ada Byron**, who devised varous programs for Charles Babbage anaytical engine. Some of them were for the General Purpose computing tools which cam out very late.

- 1930-40s - Prototypes
- 1946 - ENIAC (Electronic Numerical Integrator and Computer) was the world's first large-scale, electronic, general-purpose digital computer.
- 1971 - Microcomputers


## Machine Language

Binary numbers - 0s and 1s 
high level languages include Java, Python, c++

### **How does the translation happens?**


Source Code - What we write
Object Code - What machine understand

- Usually the process follows
Source Code -> Compiler -> Object File
-> linker -> Executable file

- In Java

Source Code -> Compiler -> Class file -> Linker -> JAR archiver -> JVM -> Run it

Why JVM is needed to execute your code when the machine is equally capable?
As all the OS speak a different version of 0s and 1s and we need a platform independent code.


## Object Oriented Language

**Why?**
It is a set of classes . Each Class is an encapsulation of behaviour/ manipulation of data.

The main class should have common characteristics and for each of its variants we can create a new sub-class. Then the variants can inherit the super class (the main class here). This is how inheritance works. 

**Objects**
Helps you access these classes by creating instances. 
Look at them as individuals that represent the classes. Like you are an object of the Human class  :)

## Variables
Has three things:
- Name
- Type
- Value

Till date, starts with a letter or underscore. 


# Operator Precednece

> In Python we follow the below:

| Precedence | Operators                                    | Associativity    | Example               |
| ---------- | -------------------------------------------- | ---------------- | --------------------- |
| Highest    | `()`                                         | —                | `(2 + 3) * 4`         |
| ↓          | `**`                                         | **Right → Left** | `2 ** 3 ** 2` → `512` |
|            | `+x`, `-x`, `~x`                             | Right → Left     | `-x`                  |
|            | `*`, `/`, `//`, `%`                          | **Left → Right** | `20 / 5 * 2` → `8`    |
|            | `+`, `-`                                     | **Left → Right** | `10 - 3 - 2` → `5`    |
|            | `<`, `<=`, `>`, `>=`, `==`, `!=`, `in`, `is` | Left → Right*    | `x < 5`               |
|            | `not`                                        | Right → Left     | `not True`            |
|            | `and`                                        | **Left → Right** | `a and b`             |
| Lowest     | `or`                                         | **Left → Right** | `a or b`              |


# Static 

A static method belongs to the class, but doesn't receive self (the object) or cls (the class).
```
class Dog:

    species = "Canine"       # class variable

    def __init__(self, name):
        self.name = name     # instance variable

    @staticmethod
    def is_dog():
        return True          # static method

```

| Concept               | Python                              |
| --------------------- | ----------------------------------- |
| Static method         | `@staticmethod`                     |
| Static/class variable | Usually called a **class variable** |
| Instance variable     | `self.x`                            |
| Instance method       | `def foo(self)`                     |


## Loop Statements
1. While Loop
2. For Loop

## Casting In Python
