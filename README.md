# Software Architecture Labs

A collection of lab exercises designed to explore core principles in software architecture, including the use of design patterns and the SOLID principles. Each lab introduces specific challenges and solutions to common architectural issues in software design, with practical examples implemented in Java.

## Table of Contents
- [Overview](#overview)
- [Lab Details](#lab-details)
  - [Lab 0: Composite and Observer Design Patterns](#lab-0-composite-and-observer-design-patterns)
  - [Lab 1: SOLID Principles](#lab-1-solid-principles)

## Overview
This repository contains two primary labs focusing on:
1. Applying design patterns to address structural and behavioral problems in software systems.
2. Adopting the SOLID principles to create more modular, maintainable, and flexible codebases.

Each lab includes problem scenarios, analysis of initial designs, and refactored solutions using design principles.

## Lab Details

### Lab 0: Composite and Observer Design Patterns
This lab demonstrates the use of the **Composite** and **Observer** design patterns to manage complex structures and notification systems.

- **Composite Pattern**: Used to manage XML-like tree structures dynamically. It addresses issues with string-based tree manipulation by allowing a unified representation of individual elements and groups of elements. This pattern enables scalable and flexible manipulation of nested structures.
  
- **Observer Pattern**: Applied to a store-customer notification system. The Observer Pattern improves efficiency by allowing customers to subscribe to specific notifications. This ensures that customers receive targeted updates on product availability without manual checking or unnecessary notifications.

### Lab 1: SOLID Principles
Lab 1 explores the five SOLID principles, refactoring initial code to enhance modularity, adaptability, and maintainability.

1. **Single Responsibility Principle (SRP)**: 
   - Refactored a `CarManager` class with multiple responsibilities into distinct classes (`CarRepository`, `CarFormatter`, `CarService`). This change improved separation of concerns and made the system more maintainable.

2. **Open-Closed Principle (OCP)**:
   - Refactored a `ResourceAllocator` class to allow new resource types without modifying existing code. Introduced a `Resource` interface, making it easier to extend functionality.

3. **Liskov Substitution Principle (LSP)**:
   - Addressed incompatibility issues in a `Duck` and `ElectronicDuck` hierarchy by defining an `IDuck` interface. This ensured that any `Duck` instance could be used interchangeably without errors.

4. **Interface Segregation Principle (ISP)**:
   - Refactored a monolithic `Door` interface into smaller, purpose-specific interfaces. This allowed classes (`SensingDoor`, `TimedDoor`) to implement only the interfaces they needed, improving modularity and readability.

5. **Dependency Inversion Principle (DIP)**:
   - Reduced coupling in an `EncodingModule` class by introducing `IDataReader` and `IDataWriter` interfaces. This decoupled high-level operations from low-level data handling implementations, increasing flexibility.

