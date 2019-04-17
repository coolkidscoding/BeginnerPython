### **Turtle Programming Commands**
---

### Introduction

Turtle graphics is a popular way for introducing programming. Virtual turtles can be programmed to move around the screen. 
The turtle draws lines as it moves. The "turtle" could look like the turtle animal, an arrow, or be invisibile. 
The user can write turtle programs that draw beautiful shapes and learn to program at the same time.

### Quickstart

```python
from turtle import *

forward(100)
left(90)
forward(100)
left(90)
forward(100)
left(90)
forward(100)
```
The instructions in your program tell the "turtle" how to move. The turtle draws a line behind it as it moves. This program draws a square. The steps given to the program are:

    Move forward 100 steps. (In the beginning, the turtle is facing to the right.)
    Turn 90 degrees to the left.
    Move forward 100 steps.
    Turn 90 degrees to the left.
    Move forward 100 steps.
    Turn 90 degrees to the left.
    Move forward 100 steps. The turtle has ended up where it started.

With these seven steps, the turtle draws a square. The from turtle import * is an instruction needed at the beginning of all of your turtle programs. It imports the turtle module so you can do the turtle instructions.

There are many instructions like left() and forward(). These instructions are called functions. This tutorial explains many of the functions in the turtle module. When you learn more of these functions, you will be able to draw many different shapes and beautiful pictures!

### Moving

By calling these functions, the turtle can be made to move around the screen. Imagine the turtle holding a pen down on the ground and drawing a line as it moves around.

The turtle's position is two numbers: the X coordinate and Y coordinate. The turtle also
forward(distance)

**forward(distance)**

The forward() function moves the turtle distance number of steps in the current direction. If the pen is down (see pendown() and penup()) a line will be drawn as the turtle moves forward. If distance is a negative number, the turtle will move backwards.
backward(distance)

**backward(distance)**

The backward() function moves the turtle distance number of steps in opposite direction the current direction. If the pen is down (see pendown() and penup()) a line will be drawn as the turtle moves backward. If distance is a negative number, the turtle will move forward.
right(angle)

**right(angle)**

The right() function will change the current direction clockwise by angle degrees. If you imagine being above the turtle looking down, the turtle turning right looks like it is turning clockwise. The turtle will not move; it will only change the direction it is facing.

**left(angle)**

The left() function will change the current direction counter-clockwise or anti-clockwise by angle degrees. If you imagine being above the turtle looking down, the turtle turning left looks like it is turning counter-clockwise or anti-clockwise. The turtle will not move; it will only change the direction it is facing.

**goto(x, y)**

The goto() function will immediately move the turtle to the given x and y coordinates. If the pen is down (see pendown() and penup()) a line will be drawn from the previous coordinates to the new coordinates.

**setx(x)**

The setx() function will immediately move the turtle to the given x coordinate. The turtle's y coordinate will stay the same. If the pen is down (see pendown() and penup()) a line will be drawn from the previous coordinates to the new coordinates.
sety(y)

**sety(y)**

The sety() function will immediately move the turtle to the given *y *coordinate. The turtle's x coordinate will stay the same. If the pen is down (see pendown() and penup()) a line will be drawn from the previous coordinates to the new coordinates.
setheading(heading)

**setheading(angle)**

The setheading() function will change the current direction to the heading angle. If you imagine being above the turtle looking down, the turtle turning left looks like it is turning counter-clockwise or anti-clockwise. The turtle will not move; it will only change the heading it is facing.

**undo()**

The undo() function will undo the turtle's last action. It will be as though the last action was never made. For example, if the last action was a call to the forward(100) function, calling undo will move the turtle backwards 100 steps and erase any line that was drawn. The undo() function can be called many times to erase more and more of the turtle

**home()**

The home() function will move the turtle to it's original position at the coordinates (0, 0) and set it's direction to 0 degrees. Calling home() is the same as calling goto(0, 0) and setheading(0). If the pen is down (see pendown() and penup()) a line will be drawn as the turtle moves back home.

### Drawing

**pendown()**

The pendown() function will cause the turtle to draw as it moves around. The line it draws can be set with the pencolor() and pensize() functions.
penup()

**penup()**

The penup() function will cause the turtle to draw as it moves around. The line it draws can be set with the pencolor() and pensize() functions.
pensize(size)

**pensize(size)**

The pensize() function sets the width of the line that the turtle draws as it moves.

**pencolor(), pencolor(color), pencolor((red, green, blue)), pencolor(red, green, blue)**

The pencolor() function sets the color of the line that the turtle draws. The pencolor() function can be passed a string of the color, such as 'red' or 'black'. Or, the pencolor() function can be passed an "RGB color triple"

**clear()**

The clear() function will erase all the line drawings on the screen. This function does not move the turtle.
reset()

**reset()**

The reset()) function will erase all the line drawings on the screen and return the turtle to the (0, 0) coordinate and facing 0 degrees. This function does the same thing as calling the clear() and home() function.