# 2.1 Design Frame

<figure><img src="../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>Flow diagram for project</p></figcaption></figure>

## Systems Diagram

This diagram shows the different parts of the project that I will focus on creating. I have split each section into smaller sub-sections. Throughout the development stage, I will pick one or two of these sections to focus on at a time to gradually build up and piece together the game. I have broken the project down this way as it roughly corresponds to the success criteria.

## Usability Features

Usability is an important aspect to my project as I want it to be accessible to all. There are 5 key points of usability to create the best user experience that I will be focusing on when developing my project. These are:

### Effective

Users can achieve the task with completeness and accuracy. To do this, I will make it easy for the users to understand what they need to do to get the most out of the app. I've mentioned this previously, about making the site simple to navigate.

#### Aims

* Make the site easy to navigate so the user can get the most from the app
* Provide sufficient information but ensure that its only essential

### Efficiency

The speed and ease of which a user can complete a task. To do this, I will create a menu system which is easy to navigate through in order for to find what you are looking for. The information which is more important can be found with less clicks.

#### Aims

* Display essential information on the home page
* Reduce the number of clicks to get to a certain feature

### Engaging

The solution is engaging for the user to use. To do this, I will implement a multitude of features which will keep users engaged with the app and willing to use it more. Using simple animations for button clicks and movements will make the website more engaging and interesting to use.

#### Aims

* Allow the user to set a goal to work towards.
* Make the site user friendly by incorporating basic website animations

### Error Tolerant

The solution should have as few errors as possible and if one does occur, it should be able to correct itself. To do this, I will write my code to manage as many different scenarios as possible so that it will not crash when someone is using it.

#### Aims

* The solution doesn't crash
* The solution does not contain any bugs that damage the user experience

### Easy To Learn

The solution should be easy to use and not be over complicated. To do this, I will create simple layout for the solution. I will make sure that no more information is added than is need, as to keep things simple for the user.

#### Aims

* It should not take more than 5 minutes to understand where you can access all the features.
* Add a basic guide to the site to make it easier to navigate.

## Pseudocode for the Solution

### Pseudocode for game

This is the basic layout of the object to store the details of the game. This will be what is rendered as it will inherit all important code for the scenes.

```
object Game
    type: Phaser
    parent: id of HTML element
    width: width
    height: height
    physics: set up for physics
    scenes: add all menus, levels and other scenes
end object

render Game to HTML web page
```

### Pseudocode for a level

This shows the basic layout of code for a Phaser scene. It shows where each task will be executed.

```
class Level extends Phaser Scene

    procedure preload
        load all sprites and music
    end procedure
    
    procedure create
        start music
        draw background
        create players
        create platforms
        create puzzle elements
        create enemies
        create obstacles
        create finishing position
        create key bindings
    end procedure
    
    procedure update
        handle key presses
        move player
        move interactable objects
        update animations
        check if player at exit
    end procedure
    
end class
```
