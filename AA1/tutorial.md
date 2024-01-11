Color the Starting Box
======================
In this activity, you will assign the player's color to the starting boxes.
<img src= "https://media.slid.es/uploads/1525749/images/10921105/pasted-from-clipboard.png" width = "100%" height = "50%">




Follow the given steps to complete this activity.




1. Color the Starting Box
* Open the file `client.py`.
* Reverse the iteration for the boxes list.
```
for box in boxes[::-1]:
```
* Assign white color to the remaining boxes except the first one.
```
if(boxes.index(box) != 0):
    box.configure(bg='white')
```


* Break the loop once the list is iterated.
```
break
```


* Save and run the code by first running the server.py and then client.py to check the output.
