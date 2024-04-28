# Snake-Game-Project
Hey, Here is the project details:

 1 – Specification

The game requires interactions with the player (e.g. the players can make choices)
The game has a graphical interface implemented using Swing.
The game should have a goal, e.g. winning condition.

The specification should include a presentation of the game, the rules, what is the goal with the game, how the user interacts with the game, and other requirements which are needed to realize the game like scoreboards. All attributes of the game should be part of the requirement specification.

 2 – Design
In this phase, you should create the object-oriented design for your game based on the requirement specification. You need to divide the functionality between the different classes. For example, the game logic and the user interface should be normally separated. Think minimalistic. Every class should have its own clear focus and a distinct goal (cohesion). Make sure to minimize dependencies between different objects (coupling).

The design phase should follow the object-oriented principles, use of inheritance, encapsulation, polymorphism and/or interface (as a pure abstract class).

3 – Implementation

The graphical interface must be responsive. In other words, the program shouldn’t freeze/deadlock, it shouldn’t be slow or jittery, and it should give clear feedback to the user.
Every class should have a clear goal and the number of dependencies should be kept low.
Methods should have a clear goal, only one goal and they should be reasonably short.
All names of functions, methods, classes, variables (i.e. all code) should be in English.
Comments should be present where it is needed, and should use English.
The code should be well-structured and easy to understand.


Test Cases that needed to be fulfilled:

A working implementation of one of the specified games has been submitted
view longer description

The game involves interactions with the player (i.e. the player needs to make choices and input those choices into the game).

The game has a graphical user interface implemented using Java Swing or JavaFX.

The implementation is object-oriented
view longer description

The solution uses encapsulation

The use of inheritance/interface must contribute to the overall OO design of your application and the child and parent classes must have an "is-a" relation.

The solution must include one interface class or one inheritance relationship that is correctly used in the code
view longer description

The code is properly formatted with consistent indentation

Suitable variable, class, and method names in English are used, with conventional capitalisation

Functional paradigm elements of Java including Lambda expressions and method references are not used.

Also, Here is are a few updates that need to be made, like:

For snake, the simplest way to create a class hierarchy to to have a class for things that go on the game board e.g. GameEntity, which has two subclasses - one for Snake and one for Food. Food can then be extended to create classes for different types of food, e.g. Apple, SuperApple and PoisonApple all of which have different effects on the snake. The Snake class can have two subclasses: SnakeHead and SnakeBody. Both have the method move(). SnakeHead can be steered by the keyboard changing a direction variable, and does the collision detection. SnakeBody can be told where to move to by its neighbour e.g. SnakeHead tells the first snake body part to move to the square the head was on. The first part tells the second and so on. If the head eats an apple it tells the body to grow - a new segment can be inserted between the head and the first body part, or the message can be passed down the body and the new segment spawned after the current last segment. fewer static methods would be an improvement. It is possible to re-implement all, apart from main(), in a non-static context.
