# Unreal Engine 5 Gameplay Systems

## Project Overview

This project showcases a collection of gameplay systems built in **Unreal Engine 5** using the **Third Person Template**. The focus is on creating modular, scalable Blueprint systems that demonstrate gameplay programming, technical design, and clean architecture.

Throughout the project, Blueprint comments have been added to explain key implementation decisions, system architecture, and design choices rather than simply describing node functionality.

---

# Implemented Features

## NPC Interaction System

A modular interaction system built using **Blueprint Interfaces**.

Features include:

* Interface-driven player interaction
* Sphere trace-based interaction detection
* Reusable interaction architecture for multiple gameplay objects
* Easily extendable to support additional interactable actors

---

## NPC Dialogue System

Implemented a simple dialogue system that allows NPCs to present dialogue through a reusable UI.

Features include:

* NPC-specific dialogue data
* Dynamic dialogue UI creation
* Dialogue loaded directly from NPC data
* Decoupled interaction and dialogue presentation

---

## NPC Waypoint System

Implemented a waypoint-based patrol system for NPCs.

Features include:

* Waypoint navigation
* Continuous patrol behaviour
* Easily configurable patrol routes
* Reusable NPC movement logic

---

## Inventory System

Implemented a modular inventory system using Actor Components and Data Tables.

Features include:

* Player Inventory Component
* Item pickup through Blueprint Interfaces
* Dynamic inventory UI
* Scroll Box populated at runtime
* Data-driven item definitions using Data Tables
* Inventory item stacking
* Quantity tracking
* Item dropping back into the world
* World pickup quantity stacking when dropping near identical items
* Individual item removal from the inventory through dropping

---

## User Interface

Implemented a simple UI to support gameplay interactions.

Features include:

* Dialogue interface
* Dynamic inventory interface
* Reusable inventory slot widgets
* Runtime population of inventory entries
* Item quantity and price display

---

# Technical Approach

The project was developed around the following technical design principles.

### Modularity

Gameplay systems are separated into reusable components and interfaces where appropriate, making them easier to expand and maintain.

### Data-Driven Design

Item definitions are stored in Data Tables, allowing values such as names, prices, icons, and pickup classes to be managed centrally rather than duplicated across multiple Blueprints.

### Reusability

Blueprint Interfaces are used to decouple player interaction from gameplay objects, allowing NPCs, pickups, and future interactables to share the same interaction workflow.

### Maintainability

Gameplay logic is centralised into reusable components to minimise duplicated Blueprint logic and simplify future feature expansion.

### Readability

Blueprints include comments explaining implementation decisions and technical reasoning to communicate the design approach behind each gameplay system.

---

# Running the Project

## Requirements

* Unreal Engine 5

## Getting Started

1. Open the project in Unreal Engine 5.
2. Load the default level if it is not already open.
3. Press **Play**.

---

# Notes

The systems in this project were designed with extensibility in mind, making it straightforward to add additional interactable objects, NPC behaviours, inventory items, and gameplay features while maintaining a modular and data-driven architecture.
