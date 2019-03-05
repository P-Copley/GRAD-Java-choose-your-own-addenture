# JAVA - Choose your own Adventure

## Goals

1. Get familiar with OOP in Java.
2. Understand type declarations and access levels.
3. Use some of the native Java data structures and their associated methods of iteration.

## Background

You may or may not have partaken in the 'Choose Your Own' genre of storybooks or computer games - either way, the concept is simple. You play a character in a certain situation, and then can choose what to do or where to go next. A classic is [The Oregon Trail](https://classicreload.com/oregon-trail.html) which was created for educational purposes, but spectacularly backfired into something entertaining, challenging and thought-provoking.

There is a sample version of a game in the solution that you can use for inspiration.

You will need the [JDK]() installed.

Any IDE will do but [IntelliJ]() is a good place to start.

A lot of the things covered in [Java101]() may be useful.

# Task

# Classes

You will use several classes in you game. Implement and test the following classes and methods.

## Player

Instances of the player class should have the following:

### Fields

- playerName : String
- fearLevel: Integer
- inventory: Array of 5 Strings.

Use the getter/setter pattern to update the fearLevel / inventory.

### Constructor

The Player constructor should take one argument, String playerName, which sets the field of playerName.

### Methods

Player should have the additional public methods: 

- stillAlive: Returns a boolean if the fearLevel is above 0.

- hasItem: Takes a string as an argument and returns true if the item is in the inventory.
 

## Room

Instances of the player class should have the following:

### Fields

- String - roomName
- String - description
- ArrayList of choices - choices

Use the getter/setter pattern to update the description / add a choice.

### Constructor

The Room constructor should take the roomName as well as an optional description.

### Methods

Rooms will need a way of comparing a players choice to the current room. Overwrite the equals method to accept a roomName as a string.
 
 
## Choice

Instances of the choice class should have the following:

### Fields

- String message
- String targetRoom
- Integer penalty - A number representing the fear a player will lose if the pick this option.
- String requiredItem - A string representing an item that is required to pick this option.
- String reward - A string representing an item the player will receive if they pick this option.


Use a combination of getter / setters and constructors to implement this class.

## Logger

-- logging methods

## Game

-- setup and play the game.