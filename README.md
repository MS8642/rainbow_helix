# rainbow_helix
# Using Python and turtle library to draw a rainbow helix.
# Note: this is a slightly updated version of the code
# from the referenced one.

# Python program to draw  
# Rainbow Benzene 
# using Turtle Programming 
import turtle 
colors = ['red', 'purple', 'blue', 'green', 'orange', 'yellow'] 
t = turtle.Pen() 
t.speed(0)
turtle.bgcolor('black') 
for x in range(360): 
    t.pencolor(colors[x%6]) 
    t.width(x//100 + 1) 
    t.forward(x) 
    t.left(59) 

turtle.done()
