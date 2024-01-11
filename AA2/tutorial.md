Color the Boxes Covered
======================
In this activity, you will color all the boxes covered by the player till the latest index position.
<img src= "https://media.slid.es/uploads/1525749/images/10921108/C115_AA2.gif" width = "100%" height = "50%">


Follow the given steps to complete this activity.


1. Color the Boxes Covered
* Open the file `client.py`.
* Create a variable to define the starting index once dice is rolled.
```
 start_index = None
```
* Assign the current index position as starting index on rolling dice.
```
start_index = boxes.index(box)
```


* Iterate through each position from the starting position to the index position for the rolled dice and color the boxes.
```
for box in boxes[start_index: steps+1]:
    box.configure(bg=color)
```


* Save and run the code by first running the server.py and then client.py to check the output.
