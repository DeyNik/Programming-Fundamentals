The lecture introduces Karel(Carol) the Robot and carry it throughout the session to teach basic coding logic, loops, and control flows..

#### What is Karel the Robot again?

Its a coding game that offers a series of levels, by clearing which, the users learn a new programming concept.
For for info check out:
https://compedu.stanford.edu/karel-reader/docs/python/en/chapter1.html

### Program Vs Algorithm:

Statements that are valid according to the syntactically according to the rules of the language.

Algorithm is the recipe for doing something

### When writing the program

1. We define a run method.
2. The run method helps executing the program by **encapsultaing** everything at one place.
3. We can then list all the intructions inside.

## How does Karel works?

1. It comes with predefined set of commands that can be executed in JAVA, Python etc (depends on what Karol version you consume)
2. It is encompassed inside a class in Java to ensure all its properties are unified and accessible from anywhere in the code.
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
- Extends ensure we get access to Karel commands like move() etc
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

while(frontIsClear()){
move();
}

### You have more conditions?

Then you have If

if(beeperPresent()){
pickBeeper();
}
else{
putBeeper();
}

and nest them

> Code should be General that fits any particular world (aka scenario).
