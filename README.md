# Unreal Engine 5 Gameplay Systems

## Project Overview

A collection of modular gameplay systems built in **Unreal Engine 5** using the **Third Person Template**. The project focuses on Blueprint architecture, reusable systems, data-driven design, and maintainable gameplay logic.

Blueprint comments document key implementation decisions and system architecture rather than simply describing individual nodes.

---

# Implemented Features

The systems below are listed in the **order they were developed**, showing the progression from foundational interaction systems to more complex, data-driven gameplay features.

## Interaction System

A reusable interaction system built with **Blueprint Interfaces**.

Features include:

* Interface-driven player interaction
* Sphere trace-based interaction detection
* Reusable interaction architecture
* Support for multiple interactable actors

---

## NPC Dialogue System

A reusable NPC dialogue system with NPC-specific dialogue data.

Features include:

* NPC-specific dialogue data
* Data-driven dialogue content
* Decoupled interaction and dialogue logic
* Reusable dialogue presentation

---

## NPC Waypoint System

A waypoint-based NPC patrol system.

Features include:

* Configurable waypoint routes
* Continuous patrol behaviour
* Reusable NPC movement logic

---

## Inventory System

A modular inventory system using **Actor Components, Blueprint Interfaces, and Data Tables**.

Features include:

* Player Inventory Component
* Interface-based item pickup
* Data-driven item definitions
* Item stacking and quantity tracking
* Item dropping
* World pickup quantity stacking
* Individual item removal

---

## Repair System

A modular repair system integrated with the inventory framework and a step-based repair workflow.

Features include:

* Removal, installation, and replacement of repair parts
* Data-driven repair workflows
* Reusable repairable object and repair-part Blueprints
* Inventory-based part validation
* Step-based repair process
* Ordered repair actions
* Example phone repair workflow:

  * Remove back cover
  * Replace battery
  * Reinstall back cover

The system separates repair data, gameplay logic, and inventory requirements, allowing new repairable objects and workflows to be added without duplicating the underlying system.

---

## Drunk System

A modular drinking and intoxication system integrated with the inventory and player gameplay systems.

Features include:

* Dedicated Drink Component
* Data-driven drink definitions
* Beer and whiskey items
* Drink status tracking
* Inventory integration
* Reusable drink Blueprints
* Configurable drink data and effects

The system is structured to support additional drinks and gameplay effects without modifying core player logic.

---

## Fast Travel System

A modular fast travel system for travelling between predefined destinations.

Features include:

* Fast Travel Point and Taxi Stand Blueprints
* Reusable Fast Travel Component
* Data-driven destination definitions
* Runtime destination population
* Third Person Character integration
* Travel audio and effects
* Extensible destination architecture

The system separates destination data and travel logic, allowing additional destinations and travel methods to be added easily.

---

# User Interface

The project includes reusable UI systems developed alongside the gameplay features.

UI functionality is separated from core gameplay logic where appropriate, allowing the underlying systems to remain reusable and maintainable.

### Dialogue UI

* Dynamic dialogue interface
* NPC-specific dialogue presentation
* Runtime dialogue content
* Reusable dialogue widgets

### Inventory UI

* Dynamic inventory interface
* Reusable inventory slot widgets
* Runtime population of inventory entries
* Item quantity and price display
* Inventory slot updates

### Repair UI

* Dynamic repair menu
* Repair step widgets
* Inventory slot integration
* Dynamic repair part selection
* Current repair step presentation
* Support for ordered repair workflows

### Fast Travel UI

* Fast travel map interface
* Dynamic destination buttons
* Runtime destination population
* Destination selection interface

### Drink Status UI

* Player drink status display
* Dynamic status updates
* Integration with the Drink Component

---

# Technical Approach

### Modularity

Gameplay functionality is separated into reusable **Actor Components, Blueprint Interfaces, Blueprints, and UI components**.

### Data-Driven Design

Gameplay data is separated from core logic using **Data Tables and reusable data structures**. This approach is used for items, destinations, repair workflows, drinks, dialogue, and other configurable gameplay data.

### Reusability

Interfaces and components reduce dependencies between systems and allow functionality to be reused across different actors and gameplay features.

### Maintainability

Common gameplay logic is centralised into reusable systems to reduce duplicated Blueprint logic and simplify future expansion.

### Readability

Blueprint comments explain important implementation decisions, architecture, and design considerations rather than simply describing individual nodes.

---

# Running the Project

## Requirements

* Unreal Engine 5

## Getting Started

1. Open the project in Unreal Engine 5.
2. Open the default level.
3. Press **Play**.

---

# Notes

The systems are designed to be **modular, reusable, and extensible**, allowing additional NPC behaviours, interactable objects, inventory items, repairable objects, fast travel destinations, drinks, UI features, and other gameplay systems to be added with minimal changes to existing systems.
