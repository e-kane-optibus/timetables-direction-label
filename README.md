# timetables-direction-label

## Purpose
This script references timetables.txt and directions.txt in feed.zip and generates a new timetables.txt with ```direction_label``` values that match the ```direction``` values in directions.txt. This is a solve for the fact that the script Support uses to generates timetables.txt for external GTFS feeds only references the first ```direction_id```:```direction``` pair in directions.txt to create ```direction_label``` values, resulting in incorrect values when there are multiple variations of the ```direction_id```:```direction``` pair.

## Usage
Tested with Python 3.9.<br>
```python3 timetables.py feed--ttable.zip``` <br>
Adjusted file is exported to the current directory as timetables_new.txt, after which the file name can be updated and added to the feed's .zip file to replace the original timetables.txt. 
