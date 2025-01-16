# Turtle-py
#i made a bird house
#1/16/25 Daily Code: Python Turtle, Flappy Bird
#Kenny 
import turtle
screen = turtle.Screen()
screen.bgcolor("light blue") 
donatello = turtle.Turtle() #donatello is mo's favorite TMNT

def square(x, y):
    donatello.pensize(12)
    donatello.pencolor("black")
    donatello.fillcolor("red")
    donatello.penup()
    donatello.goto(x, y)
    donatello.pendown()
    donatello.begin_fill()
    for i in range(4): 
        donatello.forward(390) 
        donatello.right(90)
    donatello.end_fill()

def triangle(x, y):
    donatello.pensize(12)
    donatello.pencolor("black")
    donatello.fillcolor("Brown")
    donatello.penup()
    donatello.goto(x, y)
    donatello.pendown()
    donatello.begin_fill()
    for i in range(3): 
        donatello.forward(60) 
        donatello.right(240)
    donatello.end_fill()

def star(x, y):
    donatello.pensize(6)
    donatello.pencolor("yellow")
    donatello.fillcolor("yellow")
    donatello.penup()
    donatello.goto(x, y)
    donatello.pendown()
    donatello.begin_fill()
    for i in range(12):
        donatello.forward(340)
        donatello.right(150)
    donatello.end_fill()

def circle(cx, cy, radius):
    donatello.pensize(4)
    donatello.pencolor("white")
    donatello.fillcolor("white")
    donatello.penup()
    donatello.goto(cx, cy)
    donatello.pendown()
    donatello.begin_fill()
    donatello.circle(radius)
    donatello.end_fill()
    
def hexagon(x, y):
    donatello.pensize(12)
    donatello.pencolor("black")
    donatello.fillcolor("black")
    donatello.penup()
    donatello.goto(x, y)
    donatello.pendown()
    donatello.begin_fill()
    for i in range(6): 
        donatello.forward(70) 
        donatello.right(60)
    donatello.end_fill()

#call functions
square(-180, 21)
triangle(-220, 21)
star(120, 260)
circle(-400, 250, 30)
hexagon(-20, -50)

turtle.done()
