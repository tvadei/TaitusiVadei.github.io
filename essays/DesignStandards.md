---
layout: essay
type: essay
title: "Design Standards: The Architectures of Coding"
# All dates must be YYYY-MM-DD format!
date: 2023-11-30
published: true
labels:
- Design Patterns
- Software Design
- Algorithms
- Object Oriented Programming
---

# **Design Standards: The Architectures of Coding**
As a third-year computer science student, I've transitioned from having a crack at the basics of coding to tackling more nuanced and sophisticated concepts. Among these is the field of design patterns, initially mentioned in my earlier courses, has become a key in offering numerous advantages towards my coding and software development journey. This essay is a reflection of my journey through the interesting world of design patterns. It's an exploration into what these patterns are and how they work, remodeling what was shown in my course presentations and textbooks, in an attempt to break down these concepts that often intimidate the newbies into coding. I'll also dive into my personal experiences, sharing how I've integrated design patterns into my coding assignments, and the impact this has had on my approach to writing and understanding code.

## **Understanding Design Patterns**
For many in the software development community, the 1994 book 'Design Patterns: Elements of Reusable Object-Oriented Software' symbolizes the inception of design patterns. The book, created by the ‘Gang of Four’, introduced a formalized language for discussing, analyzing and applying design patterns in an object oriented environment.

Hold on, there’s a lot to understand in that last sentence. Okay, what is a design pattern? Well, design patterns are like templates or proven solutions for common problems you often encounter when you're coding. It's like having a set of blueprints for building certain parts of your software. These solutions are not specific to one problem but can be applied to a variety of problems in similar cases. However, these aren't pieces of code that you can just copy and paste into your program. They are more like guidelines or best practices that you adapt to fit your specific needs.


Wondering what is its relationship to an object oriented environment? Design patterns are primarily based on the principles of object-oriented programming. They adhere to key OOP concepts like encapsulation, inheritance, polymorphism, and abstraction, showing us how to use these OOP principles in practical and efficient ways.

## **Application of Design Patterns**
Design patterns are broadly categorized into three main categories based on how they address different types of challenges in software development.To gain clarity, I will illustrate patterns with examples that I recall using in my Introduction to Computer Science II course where we had to use OOP methods to simulate a polynesian navigator adventure video game.

<img width="500px" height="500px" src="../img/DesignPatterns.png">

### *Category 1 - Creational Patterns*
These patterns are all about class instantiation or object creation. They help in making a system independent of how its objects are created, composed, and represented. Basically, they offer a method to make new objects without showing the detailed steps of how these objects are made, instead of making objects in the usual way with a 'new' operator. This gives the program more flexibility in deciding which objects need to be created for a given use case.

- Singleton Pattern
  This pattern ensures that a class has only one instance and provides a global point of access to it. This is useful when exactly one object is needed to coordinate actions across the system.

A use of this pattern in my video game is the Score Manager, which handles all operations related to the player's score, which is a single, global resource that should have a consistent state throughout the game. As the player finds artifacts or achieves certain objectives, the game would call addScore() to update the score.
When we need to display the score on the screen, the game would use getScore() to retrieve the current score.

- Factory Method Pattern
  This pattern defines an interface for creating an object, but lets subclasses change the type of objects that will be created. This pattern is used when a class can't anticipate the class of objects it must create.

How I implemented this is first to create the island base class. Then we create subclasses for each type of island that is visited and this would call the methods declared in the base class for example get the description of the island or get the challenge for the navigator to tackle on this island etc. Then we have the factory method class, takes an input that specifies the type of island to create and returns a new instance of the corresponding island type. Hence, when the game needs to generate a new island, it calls the factory method with the desired island type.

### *Category 2 - Structural Patterns*
Structural patterns are concerned with how classes and objects are composed to form larger structures. They help ensure that if one part of a system changes, the entire structure doesn't need to do the same. They also help in making sure that when one part of a system changes, it doesn't affect other parts of the system.

- Decorator Pattern
  This pattern is used to add new functionality to an object without altering its structure. It involves a set of decorator classes that are used to wrap components.

So the navigator's ship can be enhanced with various upgrades like faster sails, stronger armory, or special navigational equipment. We have a Ship class that has the basic functionality. Then implement a basic version of the Ship class. Then we create a Decorator class that inherits from Ship. Then we create classes for each type of enhancement, inheriting from the ShipDecorator class. Hence when the player chooses or earns an upgrade, we wrap their ship with the corresponding decorator.

### *Category 3 - Behavioral Patterns*
These patterns are all about communication between objects, how objects interact and distribute responsibility. They focus on algorithms and the assignment of responsibilities between objects. What makes them different is that they don't just describe patterns of objects or classes but also the patterns of communication between them.


- Observer pattern
  This pattern is used when an object, known as the subject, needs to notify a list of observers or subscribers when a change in its state occurs.

Since our navigators were sailing the largest ocean - the Pacific, the weather conditions can vary greatly. The weather variations have an effect on our gameplay. The weather can change from sunny, rainy, windy, stormy etc) and different parts of the game become affected such as our sailing speed, visibility and waves need to update based on the weather. Thus, whenever the weather changes (Subject), it automatically notifies all the registered Observers (player, map, enemies) about the change. These components then adjust their behavior accordingly without needing to directly check the weather state.

## **Personal Experience with Design Patterns**
Let’s reflect on how the patterns have helped me in the video game project. Using the singleton pattern helped to avoid the complexities and potential errors of multiple instances, ensuring a single, centralized and consistent resource. Similarly, the factory method created a class that acted like a central decision maker, accepting inputs and generating the required islands, streamlining the island creation process. With regards to the decorator pattern, we did not compromise the original ship class and were able to add flexibility through interchangeable objects. Pertaining to the observer pattern, game components were efficiently and instantly informed of changes to the dynamic gaming environment without having to do a constant check on the state.

Overall, the design patterns have helped me (and I’m sure countless other coders) to write clear, concise and manageable code and it is through design patterns that I am able to understand how other coders structure their work. Since it is a consistent language and widely used frame of reference, those in the community can communicate more effectively of their solutions.