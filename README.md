AbletonToUnrealOffline

Render audio / midi tracks to a CSV file for later use in Unreal Engine. 

USE: 

On the Ableton side: 
  - Drag the .amxd files onto either a midi or audio track in ableton. 
  - Just hit play and let it play. The devices will automatically record anything that's being played on the track 
  - Preview your recorded CSV file by clicking "open"
  - Write the actual file with "write", don't forget to add .csv to the file at the end when saving it to your storage device
  - hit the "clear" button if you want to start over. It will only clear the data for that track

On the Unreal side: 
  - Create a new Structure, for midi make sure you create 3 int variables and name them the same as the columns in the CSV file like this: 
![image](https://user-images.githubusercontent.com/8734041/149671645-9bea877c-2a76-4904-923f-cf106dc95ed6.png)
  - Next import the CSV file and choose your new structure as a template. 
  - Use this tutorial to generate sequencer data from the CSV file (haven't tested this part yet) 
    https://www.youtube.com/watch?v=0MKVRUvSQG8
 
NOTES:

It records everything with a build in clock, that clock runs at 30 fps. You can turn off "use heavy clock" if you want the m4l device to be less precisce but more efficient. This could be handy if you're running into CPU performance issues. 

