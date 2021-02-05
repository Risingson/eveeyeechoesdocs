# Database Sets
Create your own data sets to display on maps.
   
## Creating a set
Enter a name for the set in the input field and hit enter. 
Your set and a tab for it will get created and you will be ready to edit its details:

|  |  |
|--|--|
| Name | The name of the set is also displayed in the tabs |
| Description | Describe the data the set holds |
| Color Mode | Choose on how the data gets colored |
| Color Low | This color is used for the lowest value of the set |
| Color High | This color is used for the highest value of the set |
| Sharing | Set who can see your data (nobody by default) |
| External Data | An optional url to e.g. a google sheet |

### Individual color mode
Will color each distinct value or label with an own color. If a label and a value were entered the vlaue will be used for selecting a color automatically.

### Linear and Logarithmic color modes
Only numeric values can be colored using these modes. The lowest and highest value's colors can be set via the set's details. Other value's colors get interpolated. To understand how those modes' results look like it is best to enter some values and switch the modes. Use like 1, 2 ,3 ,4 ,5 ,10 ,20 ,50 ,1000, 5000 for seeing the difference easily.

### Color Settings
The three sliders will set Hue, Saturation and Lightness of the color used.

!!! Information "Low and high values"
    Lowest and highest values are chosen globally at the moment = If the highest or lowest values for that set are on another map those values will still be used for coloring. If you would like a mode where low and high are calculated from the displayed systems only let me know (use the [feedback forum](https://feedback.userreport.com/7ab42bbb-8bf8-4955-9573-c0b1213b1ba7/#ideas/popular) please). 
    
## Map ownership
Currently a map is owned by the user that created it originally. Also only that user can edit the map. 

## Adding Data
To add data you need to load a regional map. Opening a database set's details will show all systems on that map in a table. Edit the data and watch the map display it right away. With the details open clicking a system will sort that system to top of the list and put the cursor in the value's input field to edit right away. To bring up the normal solarsystem menu you can double-click it.

## Data Display
When opening a set's details the display options `Node` and `Label` will get activated automatically. You can  display your data via `Sectors` or `Tags` aswell. Please select them via the data displays menu. 

## Sharing maps   
Enter a discord server name you are joined on. Everybody on that server will have read only access to that set.

### Remove a map from sharing
To not share a map anymore hit `UNLINK` within the `Sharing` info line of a set's details. This will not remove the latest version from anyone who added that map but it would not get updated for them anymore. If removed by the ones using that legacy map it cannot be added back.

### Public sharing
Be aware that anybody will be able to view this dataset if you choose to make it public. 

## External Data
You can feed external data to eveeye by pasting an url to a JSON array, CSV or plain text file.
If you are using this feature you won't be able to edit data within eveeye.

### Data
The data file has to contain the following keys:

| key | description | type | max |
|--|--|--|--|
| ss | solarsystem name or id | string or numeric | - |
| lbl | label | string or numeric | 30 chars |
| val | value | string or numeric | 6 chars |

Either a label or value should be present with a solarsystem.

#### JSON Example

    [{"ss":30004738,"val":1},{"ss":"Shenda","lbl":"Hello, "},{"ss":30004271,"lbl":"3","val":"World"}]

#### CSV / TXT Example
30004738,,1<br>
Shenda,"Hello, "<br>
30004271,3,World<br>

### Google Sheets
You for example could use Google Sheets to maintain the data.
Using `File > Publish to the web` you can get the url to paste into the `External data` field:

![enter image description here](https://raw.githubusercontent.com/Risingson/eveeyedocs/master/docs/images/GS_publishCSV.png)
![enter image description here](https://raw.githubusercontent.com/Risingson/eveeyedocs/master/docs/images/GS_exampleSet.png)
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTYyNTg3Njg2Nyw1NDIxNTE1OTAsNjE1NT
I2MTY0LC0xOTM1MTUwNDU5LDEzOTM0OTY0NDgsLTI1NjUzNDk0
LC0xMTMzMjcyMDM5LDI5NjI3MTQ4OSwxNTE0NDU3MTUxLC0yMD
M5ODQ5MTQyLDU1MzA2MDUwNSwtODQ2NDk2NDI2LDE0NjI0Mzk2
ODIsMTA1ODM0MjY2NSwxNDM5MDYwNTcxLC0xMDM5OTkwMjEyLD
IzOTQwODQzLC0xODc1MzE0NTcsLTEzNjAyMjU5ODQsMjk5MDA1
MjI1XX0=
-->