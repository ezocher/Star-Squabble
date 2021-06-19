# Star Squabble - Class Design - Draft 6/21

> Note: The current version of this doc is an unorganized dump of ideas while I work out the classes for the game

---------------------

## Classes

### GameUniverse

* Turn
* List of StarSystem
    * Central list for easier rendering of map of the universe
* List of Planet
    * Central list since all planets have production and population growth every turn
    * StarSystems and Species reference Planets by ID
    * Unoccupied planets have an owner ID of 0 (Species 0)
* List of Starlane
    * Central list for easier rendering of map of the universe
* List of Ship
    * Central list since all ships in starlanes move each turn
    * Also for easier rendering of ships in map of the universe
    * Species reference ships by ID
* List of Species

### StarSystem

* List of planet IDs
* List of starlane IDs
* Orbit base time
    * Randomly set at system creation (all planets were in a line at OBT zero)
    * Planet positions easily computed as a function of orbital radius and (OBT + game time)

### Planet

* Orbital radius
* Planet type (hab or unhab or ?)
* Owner ID (none is ID of 0)
* Population - used to compute productivity (? or productivity stored and accumulated directly)
* Production, accumulated (each ship has a predetermined production cost)

### Starlane

* IDs of connected StarSystems
* Speed
* Length

### Species

Species = Player

* Name
* Homeworld

#### Visibility Lists

* List of StarSystem IDs
* List of Starlane IDs
* List of Species IDs


### Ship


