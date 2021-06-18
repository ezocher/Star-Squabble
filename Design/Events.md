# Star Squabble - Events Design - Draft 6/21

> Note: The current version of this doc is an unorganized dump of ideas while I work out the design of Events.

---------------------

## Event Categories (?name)

### Regular Event

Something that happened in the game.

Genesis events (?their own category) - creation of game universe and its components

### Utility Event

Event for the use of the game engine (e.g. Version Event).

### UI Event

Needed? - An event that triggers the appearance of specific UI.

---------------------

## Events

### Version (Utility event)

### Turn

A game turn has ended and the next one is beginning. This event increments the "wall clock" in the game.

> **Sequence of events during a turn**
>
> * All production occurs (simultaneously)
> * All interstellar ship movement occurs (simultaneously with all production)
> * All uncontested in-system ship movement occurs (simultaneously with all of the above)
> * Players receive alerts about necessary decisions, including potential combat
> * Players take actions
> * Players do turn advance button (or the turn times out)

### Genesis

A game universe has been created.

> Genesis happens on Turn 0, and players can take their first actions (e.g. setting production). Turn 1 is a regular turn with production happening at its start.

### Create System

### Create Planet

### Create TIW

### Colonize Planet

### Set Homeworld

### Set Planet Production

Sets or queues what a planet is producing. Creating a production queue of multiple items requires multiple events

---------------------

## Core Fields

### Sequence Number

The sequence number that events occurred, starting with 0. Events that occur "at the same time" all have the same sequence number. For example, all species production happens at the same time at the start of a turn.

---------------------

## Event Implementation

* Base class with common fields and subclasses for specific events
* Enumerations 

### Event Log Format

CSV file, can be viewed, edited, or created in Excel or Google Sheets.

---------------------

## Misc. Notes

* A stored Event Log could be played back to run a tutorial with special prompts and overlays triggered by events.