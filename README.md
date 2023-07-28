# Candy Crush-Flutter - A Candy Crush-like Board Game



Flutter Crush is my first ever Flutter project, developed as a board game inspired by popular match-3 games like Candy Crush, Bejeweled, and FishDom. I embarked on this project with the invaluable guidance of an online tutorial, which helped me learn the fundamentals of Flutter and implement exciting features like animations, sequences of animations, triggered animations, sounds, gesture recognition, and more.
## Table of Contents

- [Introduction](#introduction)
- [Game Mechanics](#game-mechanics)
- [Game Elements](#game-elements)
- [Objectives](#objectives)
- [Pages](#pages)
- [Screenshots](#screenshots)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Flutter Crush challenges players to create chains of at least 3 tiles of the same kind aligned either vertically or horizontally. Forming longer chains results in powerful special tiles. Players can also combine two chains with one tile in common to create impressive combos that clear large areas on the board.

## Game Mechanics

### Chains

- A chain of 3 tiles results in removing these 3 tiles.
- A chain of 4 tiles results in removing these 4 tiles, but the tile that created the chain is replaced by a TNT.
- A chain of 5 (or more) tiles results in removing all the tiles of the chain, and the tile that created the chain is replaced by a BOMB.

### Combos

- A "t" or "l" combo counts 6 tiles. All tiles of the chains are removed, and the common tile is replaced by a BOMB.
- An "L" combo counts 7 tiles. All tiles of the chains are removed, and the common tile is replaced by a WRAPPED.
- A "T" combo counts 8 tiles. All tiles of the chains are removed, and the common tile is replaced by a ROCKET.

### Bombs or Similar

- When hit, a bomb explodes, removing all tiles in the space impacted by the explosion.
- Types of bombs and their impact radius:
  - TNT: Removes tiles right next to the bomb.
  - BOMB: Removes tiles up to 2 cells around the bomb.
  - WRAPPED: Removes tiles up to 3 cells around the bomb.
  - ROCKET: Removes all tiles in its path.

### Other Elements

Additional elements may include:

- "Hole": A place where no tiles can go.
- "Wall": A place that cannot be moved nor removed from the game.
- "Ice": Covers a tile and forces the latter to be involved in at least 2 events before being removed.

## Game Elements

[Add a description here of all the different types of tiles and special elements that players can interact with.]

## Objectives

Each game level may have different objectives or a combination of several objectives, such as:

- Removal of a certain amount of a specific type of tiles.
- Creation of a certain amount of "bombs."

## Pages

### Home Page

The Home Page is the entry point of the game. It displays a beautiful background, a title, and a series of buttons, each launching a corresponding game level.

### Game Page

The Game Page contains various elements:

#### Splash Banner

At the game start, a Splash banner is displayed to show the user information related to:

- The level number
- The list of objectives

When the game is over, another Splash banner is displayed to mention whether the player won or lost the game.

#### Moves Panel

This panel is located in the top-left corner of the screen and shows the player how many moves are left before the game ends. The number of moves left is refreshed after each player's move.

#### Objectives Panel

This panel is displayed in different locations based on the device orientation:

- In portrait mode: Top-right corner
- In landscape mode: Bottom-left corner

The objectives panel consists of a series of icons representing different types of tiles and their corresponding objective counters. Each counter is refreshed whenever a player's move leads to decrementing one objective counter.

#### Board Panel

This panel displays the tiles organized based on the level definition, with dimensions depending on the device orientation and dimensions. The dimensions of a tile "square" are determined based on the device dimensions and the position of the "board."

## Screenshots



---


