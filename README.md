# Virtual Farming Game

## Overview

The Farm Management System is a simulation game that allows a player to manage a farm, including adding animals, tools, and interacting with various farm entities. This system utilizes several object-oriented programming principles, including inheritance, interfaces, method overriding, operator overloading, and more.

The game lets the player manage different types of animals (cow, chicken, sheep), track inventory, and perform tasks like harvesting and combining tools.

---

## Features

- **Player Management**: A player can manage a farm, add animals, tools, and farm entities.
- **Animal Production**: Each animal (Cow, Chicken, Sheep) can produce different goods.
- **Tool Inventory**: Tools can be added to the player's inventory, with limits.
- **Static Fields and Methods**: Track the total number of animals across the entire game.
- **Operator Overloading**: The player can combine tools using the overloaded `+` operator.
- **Inheritance and Interfaces**: Animal entities inherit from a base class and implement the `IProduce` interface.

---

## OOP Features and Implementation

| **OOP Feature**         | **Implementation Details**                                                                                  | **Where Implemented**                                      |
|-------------------------|--------------------------------------------------------------------------------------------------------------|------------------------------------------------------------|
| **Function Overloading** | Methods `AddTool` are overloaded to accept either one or two tools.                                         | `Inventory` class (`AddTool` method)                       |
| **Constructors**         | The `Player`, `Animal`, `Tool`, `Cow`, `Chicken`, `Sheep` classes have constructors to initialize properties. | `Player`, `Animal`, `Tool`, `Cow`, `Chicken`, `Sheep` classes |
| **Constructor Overloading** | Multiple constructors are provided for `Player` class (one for new player and one for copy constructor). | `Player` class (Constructor and Copy Constructor)          |
| **Operator Overloading** | The `+` operator is overloaded in the `Tool` class to combine two tools.                                     | `Tool` class (`+` operator)                               |
| **Static Methods**       | The `TrackAnimal` method is static and keeps track of the total number of animals created.                  | `Player` class (`TrackAnimal` method)                      |
| **Static Fields**        | The `AnimalCount` field is static and tracks the total number of animals across all `Player` instances.     | `Player` class (`AnimalCount` field)                       |
| **Classes**              | Multiple classes are used to model the farm system: `Player`, `FarmEntity`, `Animal`, `Cow`, `Chicken`, `Sheep`, `Tool`, `Inventory`. | `Player`, `FarmEntity`, `Animal`, `Cow`, `Chicken`, `Sheep`, `Tool`, `Inventory` classes |
| **Copy Constructors**    | The `Player` class contains a copy constructor to create a new player by copying an existing player.         | `Player` class (Copy Constructor)                          |
| **Inheritance**          | `Animal` inherits from the abstract `FarmEntity` class. `Cow`, `Chicken`, and `Sheep` inherit from `Animal`. | `FarmEntity`, `Animal`, `Cow`, `Chicken`, `Sheep` classes  |
| **Interfaces**           | The `IProduce` interface is implemented by the `Animal` class and its subclasses to define a `Produce` method. | `IProduce` interface implemented in `Animal` class         |
| **Method Overriding**    | The `Produce` method is overridden in `Cow`, `Chicken`, and `Sheep` to provide specific behaviors for each animal. | `Cow`, `Chicken`, `Sheep` classes (`Produce` method)      |
| **Virtual Methods**      | The `Produce` method is declared as virtual in the `FarmEntity` class, allowing overriding in derived classes. | `FarmEntity` class (`Produce` method)                     |
| **Abstract Classes**     | The `FarmEntity` class is abstract, defining methods that must be implemented by subclasses.                | `FarmEntity` class (abstract)                             |

---

## Project Information

- **Uttara University**
- **Team Name**: Team Notepad++
- **Faculty Name**: Nahrin Jannat
- **Course Name**: Object Oriented Programming
- **Project Type**: Lab Final Project
- **Group Members**:
  - **Member 1**: NAZMUL HAQUE HIMU, 2233081403
  - **Member 2**: [Name], [ID]
  - **Member 3**: [Name], [ID]
  - **Member 4**: [Name], [ID]
  - **Member 5**: [Name], [ID]

---

## Setup and Usage

1. **Clone the repository** or **Download the source code** to your local machine.
2. **Open the project** in Visual Studio (or your preferred C# IDE).
3. Build and run the project to start the simulation.
4. The player will be prompted to manage farm entities like animals and tools.

---

## Example Output

