Set the Dice and Player Color
======================
In this activity, you will define a function to update the player's position on the game board based on the dice value and the color assigned to a player.
<img src= "https://media.slid.es/uploads/1525749/images/10918961/C115_SA2.gif" width = "100%" height = "50%">




Follow the given steps to complete this activity.




1. Add and fetch the transactions from the database
* Open the file `client.py`.
* Configure the die color if the player turn exists using the canvas2.itemconfigure() method.
```
if('player2_turn' in message):               
    canvas2.itemconfigure(dice, fill="yellow")
```




* Set the boxes to the left or right to move the player by checking the color within an user-defined function.
```
def move_player(steps, color):
    global left_boxes, right_boxes
    if(color == 'yellow'):
        boxes = right_boxes
```
* Move the player by calling the move_player() function with dice_value as first parameter and configure the box color by passing "yellow" as the second parameter.
```
move_player(dice_value, 'yellow')
```




* Select the box using index steps and configure its background color to that of the player's color.
```
boxes[steps].configure(bg=color)
```


* Save and run the code by first running the server.py and then client.py to check the output.
