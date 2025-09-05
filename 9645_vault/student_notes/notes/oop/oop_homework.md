02/09/2025

# Notes
### Definitions
- **Inheritance**: when classes (subclasses) inherit data and behaviour from a parent class (superclasses)
- **Association**: classes can be associated with each other, e.g. how a railway company would be associated with engines -> however, there is no ownership between the objects
- **Aggregation**: a specific type of association, which occurs when a class contains other classes that don't depend upon the container, e.g. a player in a team does not die if the team is disbanded
- **Composition**: a stronger form of association, where if the container is destroyed, every instance of the contained classes are also destroyed, e.g. if a hotel is destroyed all the rooms are too
- **Polymorphism**: a programming language's ability to process objects differently depending on their class
- **Interface**: a collection of abstract methods that a group of unrelated classes may implement

### Access modifiers (public, private and protected)
**Information hiding** is where an objects instance variables are hidden so that other objects must use messages to interact with that object's state. **Public**, **private** and **protected** are included in class definitions to implement data hiding. 
- **Private** methods/variables - only code within the class can access them
- **Public** methods/variables - code within any class can access them
- **Protected** methods/variables - (definition varies between languages)
*Instance variables are usually declared private and methods public, so other classes cannot change variable values but can use methods*

| Member is accessible:                     | Public | Protected          | Private |
| ----------------------------------------- | ------ | ------------------ | ------- |
| Within defining class                     | Yes    | Yes                | Yes     |
| Via inheritance                           | Yes    | Yes                | No      |
| Via a reference to an object of the class | Yes    | Only in some cases | No      |

### Interfaces
Where methods are created - methods can be implemented into any class that the programmer wishes them to be used in. 

### Advantages of OOP
- Forces designers to do extensive planning -> better designs with fewer weaknesses
- Encapsulation: source code for an object can be written, tested, and maintained independently of code for other objects
- Knowledge of how methods are implemented into an object is not necessary for it to be used
- New objects with small differences to other ones can be easily created
- Re-usability: objects that are already defined, coded, and tested can be used in many different programming
- Software maintenance: an object oriented program is easier to maintain than one written in a procedural language due to its rigidly enforced modular structure

# Questions

Q1) 
- a: aggregation
- b: composition
- c: aggregation
Q2)
Tom would move three spaces to the right, while Jerry would move two spaces to the right
Q3)
Override the move two spaces method so that beavers only move one space

# Exercises
1)
	a. Inheritance is where subclasses inherit the ability to use/access objects made in parent classes 
	b. ??
	c. When a method is defined that has the same name and arguments as a method inherited from a superclass
	d. 
``` python
class MusicFile:
	artist = ""
	sample_rate = 0
	bit_depth = 0
```
2)
	a. Polymorphism is the concept where you can access objects of different classes through one interface
	b. 
		i) bird1.move will output "Birds can fly", bird2.move will output "Seagulls can fly and swim"
		ii) This is because although Seagull is within the class Bird, the move procedure has been overrided so it will perform a different action than in Bird. 
3)
	a. Aggregation is where a class contains other subclasses that do not depend on the superclass
	b. 
``` python
Class Table:

Class Chair:

Class GardenSet:
	TableType = ""
	ChairType = ""
	NumberOfChairs = 0
	def DisplayDetails(self):
		self.__table_type = TableType
		self.__chair_type = ChairType
		self.__num_chairs = NumberOfChairs
```
	c. The private access modifier means that only code within the defining class can access the method/variable. The public access modifier means that the method/variable can be accessed from anywhere in the program. Variables are usually declared private so other classes cannot change the values, but methods are public so that they can be used anywhere. 