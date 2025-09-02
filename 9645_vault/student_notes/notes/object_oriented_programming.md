02/09/2025

# Notes
### Definitions
- **Association**: classes can be associated with each other, e.g. how a railway company would be associated with engines -> however, there is no ownership between the objects
- **Aggregation**: a specific type of association, which occurs when a class contains other classes that don't depend upon the container, e.g. a player in a team does not die if the team is disbanded
- **Composition**: a stronger form of association, where if the container is destroyed, every instance of the contained classes are also destroyed, e.g. if a hotel is destroyed all the rooms are too
- **Polymorphism**: a programming language's ability to process objects differently depending on their class

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


# Questions

Q1) 
- a: aggregation
- b: composition
- c: aggregation
Q2)
Tom would move three spaces to the right, while Jerry would move two spaces to the right
Q3)
Override the move two spaces method so that beavers only move one space