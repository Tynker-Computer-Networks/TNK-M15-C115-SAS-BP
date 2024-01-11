Color the Current and Finishing Box
======================
In this activity, you will recolor the previous position boxes and color the current position box.
<img src= "https://media.slid.es/uploads/1525749/images/10918522/C115_SA3.2.gif" width = "100%" height = "50%">




Follow the given steps to complete this activity.




1. Color the Current and Finishing Box
* Open the file `client.py`.
* Iterate through each box using a for loop to reach the previous position of the player.


* Check if the background color matches with that of the player color for the previous box index using .cget() method to retrieve the background color.


* Configure the background color for the previous position.


* Configure the background color for the current box by incrementing the steps by adding the index position.
```
for box in boxes:
    if(box.cget("bg") == color):
        box.configure(bg='white')
        steps += boxes.index(box)
```


* Save and run the code by first running the server.py and then client.py to check the output.
