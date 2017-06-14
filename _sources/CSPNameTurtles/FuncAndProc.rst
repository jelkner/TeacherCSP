..  Copyright (C)  Mark Guzdial, Barbara Ericson, Briana Morrison
    Permission is granted to copy, distribute and/or modify this document
    under the terms of the GNU Free Documentation License, Version 1.3 or
    any later version published by the Free Software Foundation; with
    Invariant Sections being Forward, Prefaces, and Contributor List,
    no Front-Cover Texts, and no Back-Cover Texts.  A copy of the license
    is included in the section entitled "GNU Free Documentation License".

.. |bigteachernote| image:: Figures/apple.jpg
    :width: 50px
    :align: top
    :alt: teacher note

.. 	qnum::
	:start: 1
	:prefix: csp-5-2-
	
.. highlight:: java
   :linenothreshold: 4

Procedures and Functions
================================

We have seen string **functions** like ``lower()`` which returns a new string with all lowercase characters.  **Functions** return a value.  The ``Screen()`` and ``Turtle()`` in the code below both create objects and return them, so they are functions.   You can also have **procedures** which do some action, but don't return anything.  The ``forward(75)`` and ``left(90)`` below are both procedures since they do an action, but don't return anything. 

.. note::
   Some Python books don't make a distinction between procedures and functions and will call both of these functions.  In this book we are using **function** only for named code that returns a value and **procedure** for named code that doesn't return a value.   
   

   
.. fillintheblank:: 5_2_1_LetterC_fill

    .. blank:: 5_2_1_LetterC
        :correct: ^c$|^C$
        :feedback1: ('.*','Try to follow the directions as if you are the turtle')

        What letter (like A and D) will the program below draw in block style when you click on the Run button?

.. activecode:: Turtle_C
    :nocodelens:
	
    from turtle import *    # use the turtle library
    space = Screen()        # create a turtle space
    alex = Turtle()         # create a turtle named alex
    alex.left(180)          # turn alex by 180 degrees
    alex.forward(75)        # move forward by 75 units 
    alex.left(90)           # turn left 90 degrees
    alex.forward(100)       # more forward by 100 units
    alex.left(90)           # turn left 90 degrees
    alex.forward(75)        # move forward by 75 units 
    
**Check Your Understanding**

.. mchoice:: 5_2_2_FuncOrProc
   :answer_a: function
   :answer_b: procedure
   :correct: b
   :feedback_a: Does it return a value?
   :feedback_b: The right procedure will cause the turtle to turn right by the specified number of degrees and doesn't return any value so it is a procedure.

   Is right(90) a function or procedure?
    
.. note ::

   In these next problems we will draw a letter similar to how you might do it without lifting your pen or pencil.    See the numbers and arrows on the letters for the order that the lines are drawn.
    
**Mixed up programs**

.. parsonsprob:: 5_2_1_Turtle-T
   :adaptive:

   The following program uses a turtle to draw a capital T as shown to the left, <img src="../_static/TurtleT1.png" width="150" align="left" hspace="10" vspace="5"/> but the lines are mixed up.  The program should do all necessary set-up, create the turtle.  After that the turtle should turn to face north, draw a line that is 150 pixels long, turn to face west, and draw a line that is 50 pixels long.  Next, the turtle should turn 180 degrees and draw a line that is 100 pixels long.<br /><br /><p>Drag the blocks of statements from the left column to the right column and put them in the right order.  Then click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order.</p>  
   -----
   from turtle import *
   =====
   space = Screen()    	
   jamal = Turtle()
   ===== 
   jamal.left(90)
   =====                
   jamal.forward(150)
   =====
   jamal.left(90)
   jamal.forward(50)
   =====
   jamal.right(180)
   =====
   jamal.forward(100)
   
**Mixed up programs**
   
.. parsonsprob:: 5_2_2_Turtle-A

   The following program uses a turtle to draw a capital A as shown to the left, <img src="../_static/turtleA2.png" width="150" align="left" hspace="10" vspace="5"/> but the lines are mixed up.  The program should do all necessary set-up, create the turtle.  After that the turtle should turn left 70 degrees, draw a line that is 100 pixels long.  Next it should turn right 135 degrees and draw another line that is 100 pixels long.  Then the turtle should reverse direction and draw a line 50 pixels long.  And finally it should turn left 65 degrees and draw the line between the other two lines.  .<br /><br /><p>Drag the blocks of statements from the left column to the right column and put them in the right order.  Then click on <i>Check Me</i> to see if you are right. You will be told if any of the lines are in the wrong order.</p>  
   -----
   from turtle import *
   space = Screen()  
   =====  	
   jamal = Turtle()
   ===== 
   jamal.left(70)
   =====                
   jamal.forward(100)
   jamal.right(135)
   =====
   jamal.forward(100)
   =====
   jamal.right(180)
   =====
   jamal.forward(50)
   =====
   jamal.left(65)
   jamal.forward(45)


