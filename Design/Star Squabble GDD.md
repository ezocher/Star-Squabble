# Star Squabble - Game Design Document

## Description

*"Risk" in Space*

A multiplayer turn-based 4X strategy game with units and combat inspired by Risk and with a 3D star map and traversable interstellar wormholes inspired by Ascendancy's starlanes.

Controlling territory is the primary objective like Risk, but there is also the traditional 4X "fog of war" where each player can only see the area that they've explored.

## Project Objectives

Develop a streamlined and visually simple game to focus on the gameplay, strategy, AI, and game architecture.

## Backstory

In a faraway elliptical galaxy, a cluster of stars formed from a dense molecular cloud. Conditions were nearly perfect, and the cluster was eventually teeming with life. An incredible diversity of forms had evolved on more than two dozen planets, and in two cases, consciousness had been achieved.

Sadly, before the /Bezzi and the Hommm had managed to contact one another, they both discovered that the massive blue star (120 solar masses) at the center of the cluster was becoming unstable and the Hommm had deduced that it was about to go supernova.

When the explosion came … *TBD*

On fifteen of the worlds, the hardiest microscopic life managed to survive in the crust and deep oceans of the planets.

Life, as it is prone to do, started again on its long evolutionary journey.

We pick up our story 1.5 billion years later. Sentient species have emerged on ten of the worlds and they are beginning to explore and colonize their solar systems. You are the supreme leader of one of those species.

# Gameplay

## Core Elements

### Star Systems

Star Systems have one star and one or more planets.

### Planets

Planets are habitable or challenging (toxic/too hot/too cold/etc.). Planets can be uninhabited or colonized.

Colonies on habitable planets can begin production as soon as they are founded. Colonies on challenging worlds begin terraforming at founding and when terraforming is complete they begin production.

Production slowly increases as population grows. ?? Production can be increased more quickly by building production instead of ships.

A planet can be colonized by a single ship of any size. The personnel from the ship become colonists and the ship's material is used in the founding of the colony. Larger ships will start a colony with a greater population, which results in a higher production rate at founding than a smaller population would provide.

Planets produce ships.

If a fleet of ships eliminates all enemy ships in a system, then on the next turn they can choose to attempt invasion of one or more planets in the system (see combat below).

In an unsuccessful invasion, the invading ship(s) are lost. In a successful invasion 

### Ships

Ships come in 4 sizes and are either in-system ships or interstellar ships. The sizes are patrol (1 ship unit), destroyer (2 units), cruiser (4), and dreadnought (8).

Ships can explore other star systems (interstellar ships only), colonize empty planets, fight space battles versus other ships, or invade other species' planets (taking over their colonies).

In-system ships can be built in any size and cost 50% of an interstellar ship of the same size. In-system ships cannot travel among the stars but can colonize planets in the system, invade planets in the system, or act as defense for a system.

Ships entering a system where there are ships from other species can choose to flee or engage. Ships already in a system can also choose to flee or engage.

### TIWs - Traversable Interstellar Wormholes

Two flavors: regular and long/slow

### Sectors

Star systems connected by regular TIWs constitute a sector



# Game Architecture

## Core Architecture Principles

* Separated and pluggable UI
* Event-driven architecture
* Pluggable AI - Open and pluggable AI per player to enable rapid experimentation


## Event-based architecture

### Description

### Objectives

### Benefits

# Project

## Engine, Libraries, Services, Tools

* C# (version ?)
* Unity 20??


## Team

* Eric Zocher