
# Exp.No:28  
## Abstraction

### AIM  

To Create an abstract base class has a concrete method sleep() that will be the same for all the child classes. So, we do not define it as an abstract method, thus saving us from code repetition. On the other hand, the sounds that animals make are all different. For that purpose, define the sound() method as an abstract method. then implement it in all child classes.

### ALGORITHM
1.	Start
2.	Import the required module:
    - Import ABC and abstractmethod from the abc module to define an abstract base class.
3.	Define the abstract base class:
4.	Name it Animal.
5.	Create a concrete method sleep() that prints "I am going to sleep in a while".
6.	Define an abstract method sound() using the @abstractmethod decorator. This method will be overridden in subclasses.
7.	Define a subclass (e.g., Cat) that inherits from Animal:
8.	Implement the sound() method in the subclass to print:
a.	"I can meow"
b.	"I can hiss"
9.	Create an object of the subclass (e.g., Cat).
10.	Call the methods:
11.	Call sleep() to display the common sleep message.
12.	Call sound() to display cat-specific sounds.
13.	End



### PROGRAM

```

from abc import ABC, abstractmethod

# Abstract Base Class
class Animal(ABC):
    def sleep(self):
        print("I am going to sleep in a while")

    @abstractmethod
    def sound(self):
        pass

# Child Class
class Cat(Animal):
    def sound(self):
        print("I can meow")
        print("I can hiss")

# Example usage
c = Cat()
c.sleep()
c.sound()

```

### OUTPUT

![image](https://github.com/user-attachments/assets/ea81dcc9-f5f5-4b2c-8aa6-712ef4c81dd8)


### RESULT

Thus the python program for abstract method was successfully created.
