Color the Current and Finishing Box
======================
In this activity, you will use a flag variable updated to color the current box only if the step index is less than that of the length of the box. On reaching the finishing box, we will color the box to that of the winning player color.
<img src= "https://media.slid.es/uploads/1525749/images/10918522/C115_SA3.2.gif" width = "100%" height = "50%">




Follow the given steps to complete this activity.




1. Color the Current and Finishing Box
* Open the file `client.py`.
* Set the flag variable to 'false' to further color the current box.
```
updated = False
```
* Move the player piece only when the next index position is less than equal to the length of the boxes and then update the flag variable to 'true'.
```
if(box.cget("bg") == color and steps+boxes.index(box) <= len(boxes)):
    box.configure(bg='white')
    steps += boxes.index(box)
    updated= True
```


* Update the color of the current index box only if the value of the flag variable is 'true'.
```
if(updated):
    print("Updated", steps)
    boxes[steps].configure(bg=color)
```


* Update the color of the finishing box to that of player color when the steps covered are equal to that of the length of the boxes.
```
if(steps==len(boxes)):
    finishing_box.configure(bg= color)
    updated=False
```


* Save and run the code by first running the server.py and then client.py to check the output.
