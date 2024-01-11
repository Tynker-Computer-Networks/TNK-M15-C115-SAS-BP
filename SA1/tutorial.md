Print the Value on Dice
======================
In this activity, you will roll the dice and display the value on the dice face.
<img src= "" width = "100%" height = "50%">




Follow the given steps to complete this activity.




1. Print the Value on Dice
* Open the file `client.py`.
* Set the value for the faces on the dice for a rolled dice.
```
if('\u2680' in message):
    canvas2.itemconfigure(dice, text='\u2680')
    dice_value = 1
elif('\u2681' in message):
    canvas2.itemconfigure(dice, text='\u2681')
    dice_value = 2
elif('\u2682' in message):
    canvas2.itemconfigure(dice, text='\u2682')  
    dice_value = 3
elif('\u2683' in message):
    canvas2.itemconfigure(dice, text='\u2683')
    dice_value = 4
elif('\u2684' in message):
    canvas2.itemconfigure(dice, text='\u2684')
    dice_value = 5
elif('\u2685' in message):
    canvas2.itemconfigure(dice, text='\u2685')
    dice_value = 6
```


* Print the value on the face of the rolled die using the print() method.
```
print("Dice value: ", dice_value)
```


* Save and run the code by first running the server.py and then client.py to check the output.
