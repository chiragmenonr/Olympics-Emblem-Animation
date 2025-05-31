# Olympics-Emblem-Animation
When the program is run, a turtle will draw the Olympics emblem along with the corresponding colors

import turtle # Allows to use the turtle

wn = turtle.Screen()
oly = turtle.Turtle() # sets the variable for the turtle

oly.hideturtle() # Hiding the ugly turtle from sight

oly.speed(0) # The speed at which the emblem is made

oly.pencolor("blue") # Setting the initial color to blue

oly.penup() # going back to allow the turtle more space to put the emblem
oly.back(200)
oly.pendown()

for rowOne in range(3): # A for loop to print three circles

		for c in range(100): # A for loop with the instructions to make each circle
        oly.forward(4)
        oly.left(3.6)
        oly.pensize(8)

    oly.penup() # Code to allow the turtle to start working on the next circle
    oly.forward(150)
    oly.pendown()

    if oly.pencolor() == "blue": # If the color is blue,
        oly.pencolor("black") # ...then change it to black
    else: oly.pencolor("red") # Otherwise, change it to red
        

oly.penup() # Going down to make the two circles on the bottom
oly.back(375)
oly.right(90)
oly.forward(50)
oly.left(90)
oly.pendown()

for rowTwo in range(2): # A for loop to print two circles

    if oly.pencolor() == "red": # If the color is red,
        oly.pencolor("orange") # ...then change it to orange
    else: oly.pencolor("green") # Otherwise, change it to green

    for m in range(100): # A for loop with the instructions to make each circle
        oly.forward(4)
        oly.left(3.6)
        oly.pensize(8)
    oly.penup() # Code to allow the turtle to start working on the next circle
    oly.forward(150)
    oly.pendown()

wn.mainloop() # The end of the code
