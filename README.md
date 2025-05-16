# LuaMapTest

**Dream Editor** project showcasing game development concepts utilizing Lua scripting and JSON data configuration within the Dream Editor environment. This project implements fundamental gameplay mechanics, including distinct hero and enemy units, abilities, dynamic enemy spawning, a scoring system, and an in-game upgrade mechanism.

### Key Features:

* **Lua-Scripted Gameplay Logic:**
    * Game event management (map start, unit death, key presses) handled through Lua triggers.
    * Dynamic spawning and control of a player-controlled "Hero FireMage" unit and AI-controlled "Hero IceMage" enemy units.
    * Implementation of unique abilities for units, such as "Delayed Blast Fireball" for the FireMage and "Ice Spike" for the IceMage, defined in `Ability.json` and triggered via Lua.
    * A scoring system that increments as enemy units are defeated.
    * An interactive UI button that triggers an upgrade for all active enemy units, enhancing their damage and maximum health. 
    * Comprehensive use of JSON files to define and manage game entities and their properties:
        * **Abilities (`Ability.json`):** Defines spell effects, casting parameters, costs, and target filters.
        * **Actors (`Actor.json`):** Configures visual and audio resources for units and abilities, including models, particle animations, and sound effects.
        * **Behaviors (`Behavior.json`):** Specifies status effects and modifications, like the "Damage and MaxHealth Increase 10%" upgrade. 
        * **Effects (`Effect.json`):** Details the outcomes of abilities and actions, such as damage application and area searches.
        * **Movers (`Mover.json`):** Controls the movement patterns of projectiles like "Delayed Blast Fireball Missile." 
        * **Units (`Unit.json`):** Defines the stats, components (health, mana, movement), and abilities/weapons of game units.
        * **Weapons (`Weapon.json`):** Configures weapon properties, such as the "Hero IceMage Weapon."
        * **Terrain (`Terrain.json`):** Describes the map layout, tile data, and lighting. 
* **Object-Oriented Programming in Lua:**
    * The `Assets/Scripts/Inheritance.lua.txt` file demonstrates OOP principles in Lua with base classes like `ScoreCounter` and `GameUnit`, and a `Hero` class inheriting from `GameUnit`. This showcases modular design for game entities and systems.
    * Includes examples of deep and shallow copy mechanisms for objects.
* **Custom User Interface:**
    * A simple UI is defined in `UI.xml`, featuring an "Upgrade Enemies" button.
    * Interaction with this UI element is handled in `Trigger.lua.txt` to apply upgrades to enemy units. [cite: 14]

### Technologies Used:

* **Lua:** For all core gameplay scripting and logic.
* **JSON:** For data configuration of all game assets and entities.
* **Dream Editor:** The development environment for which this project is intended.
* **XML:** For UI definitions (`UI.xml` and basic trigger structure `Trigger.xml`).

### Relevance for Resumes:

This project demonstrates capabilities in:

* **Lua Scripting:** Proficiently applied Lua for game logic, event handling, ability implementation, and AI behavior.
* **Data-Driven Development:** Effectively utilized JSON to manage complex game data, allowing for flexible and scalable game design.
* **Gameplay Mechanics Implementation:** Successfully developed core gameplay features including unit control, combat abilities, enemy wave management, scoring, and dynamic upgrade systems.
* **Object-Oriented Principles:** Applied OOP concepts in Lua to create organized, reusable, and maintainable code for game objects and systems.
* **Game Asset Configuration:** Managed and configured various game assets including actors, visual effects, sound effects, and unit properties through data files.
* **Custom UI Development:** Implemented basic UI elements and their corresponding backend logic for player interaction.
* **Version Control/Project Structure:** Maintained an organized project structure with clear separation of data, scripts, and assets.
