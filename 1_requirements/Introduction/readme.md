# Introduction
Snake Game is the classic video game concept where the player maneuvers a line which grows in length, with the line itself being a primary obstacle The player controls a dot, square, or object on a bordered plane.

As it moves forward, it leaves a trail behind, resembling a moving snake. In some games, the end of the trail is in a fixed position, so the snake continually gets longer as it moves.

In another common scheme, the snake has a specific length, so there is a moving tail a fixed number of units away from the head.

The player loses when the snake runs into the screen border, other obstacle, or itself.

Snake game is a classic computer action game, in which we control a snake to move and collect food in a map.

Which has been arround since the earliest days of home computing, and has re-emerged in recent years on mobile phones it isn't world's greatest game, but it does give you an idea of what you can achieve with relatively simple c program, and perhaps the basis by which to extend the principles. it can create more intresting games of your own.

# GamePlay
The game environment is a 30030 map. The snake starts with length one.

At each time step the snake moves one step, and it can go straight, turn left, or turn right

The snake hits its own body or the wall, The length of the snake gets zero, The game score gets negative.

The Main aim of the game is to collect the dots(Food) and avoid the obstacles (boarders, crosses, and the snake itself). As you collect the food, the snake gets longer , so increasing your likelihood of crashing into yourself. when you collected enough food, you progress into the next level, where your snake gets larger.

you get scored according to the length of the snake and the no. of 'x' obstacles in the screen. The speed increases every 5 levels. you get a bonus when you complete the level of 1000.

History of the game
The Snake design dates back to the arcade game Blockade, developed and published by Gremlin in 1976. It was cloned as Bigfoot Bonkers the same year. In 1977, Atari, released two Blockade-inspired titles: the arcade game Dominos and Atari VCS game Surround. Surround was one of the nine Atari VCS launch titles in the US and was sold by Sears under the name Chase. That same year, a similar game was launched for the Bally Astrocade as Checkmate.

Snake II was launched with Nokia’s 3310 in 2000 and it became an entire generation’s obsession. The snake wasn’t just a line anymore, but had a proper form, there were bonuses and the screen was cyclical, allowing one to go through the bottom of the screen and come back out the top. In India and across the world, kids were hooked, eagerly competing for the highest score whether they were lying in bed, pretending to study in class or sitting at a café. Draining a phone’s battery and earning the wrath of exasperated teachers was just collateral damage. An addictively simple game, Snake was launched, in its mobile phone avatar, in 1997 with the Nokia 6110 — you remember, the blue candy bar-shaped model with a single antenna

Software requirements
Software Requirements: OPerating system : WINDOWS 8/9/10 Application Software: TURBO C++ 2.0 Language: C computer graphics Hardware Requirements: Hard disk : 32GB RAM: 128MB processor : Any pentium Version

Many functions have been used in this Snake Game . Here, I will just list them below and describe the functions “gotoxy”, “GotoXY” and “delay” as they are some of the most important functions

void record() void load() void Delay(long double) void Move() void Food() void Print() void Bend() int Score() void Boarder() void Down() void Left() void Up() void Right() void ExitGame()

# Features
Features & About the Project? *This snake game is just similar to games which are found under mobile games section. It uses the concept of graphics to display the menu items and all objects on a single screen.

*An instruction has been given on the top right side of the menu where users must go through the instruction to play this game.

*Players will able to check their result after games get over.

*The score section will display the total score of the player, game level maze which has been used.

*The object snake position has been set random, so whenever player will Start the game, the snake will appear at random location every time.

*The snake object will always appear in WHITE color. The ARROW keys "UP,DOWN,RIGHT,LEFT" has been set within the program to move the snake to right, left, top and bottom respectively

# FUTURE SCOPE
Our project will be able to implement in future making some changes and modifications as we make my project at a very low level. So the modifications that can be done in my project are:

after

1.It can be made with good graphics.

2.We can add more options like Top scores and Player Profile

3.We can add multiplayer option

# CONCLUSION
This Project in C language of Snake Game is a simple console application with very simple graphics. In this project, you can play the popular "Snake Game" just like you played it elsewhere. You have to use the up, down, right or left arrows to move the snake.

Foods are provided at the several co-ordinates of the screen for the snake to eat. Every time the snake eats the food, its length will by increased by one element along with the score. It isn't the world's greatest game, but it does give you an idea of what you can achieve with a relatively simple C program, and perhaps the basis by which to extend the principles and create more interesting games of your own.

Reference
https://en.wikipedia.org/wiki

Books
1.Programming with C by E Balagurusamy

2.Graphics under C by Yashwant
