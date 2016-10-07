I really hope that you will enjoy this book and have fun with your kids. 
Feel free to share your experiences with me ducasse@iam.unibe.ch

The directory contains some possible solutions of the experiments I proposed, I strongly encourage you to play and experiment with the environment to create your own problems and solution. 

15 July 2005 - StŽphane Ducasse




Here is a list of fixes due to typos.

Chapter 16 p 192, 

goldenRectangle: widthSize atLevel: n 
   "Draw n + 1 golden rectangles whose bigger one is of widthSize width"

   | currentRectangleWidth |
    currentRectangleWidth := widthSize.
    self goldenRectangle: currentRectangleWidth.
    n timesRepeat:
            [ self parallelWidthSegment: currentRectangleWidth.
            self turnLeft: 90.
            currentRectangleWidth := currentRectangleWidth * (((1 + 5 sqrt) / 2) - 1)]
            
Chapter 16 page 193, 
currentRectangleWidth := currentRectangleWidth * (((1 + 5 sqrt) /2 -1)            


p 223

In figure 19-2

[ self center y > 100 ]
	whileTrue: [ self go: 10 ]