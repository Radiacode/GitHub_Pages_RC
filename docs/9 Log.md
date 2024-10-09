This page displays the current and past measurement data in a table. As new meaningful data becomes available, it is added to the log.

![Log](Images/log.png)

Above the table, there are icons for filter types of measurements and events and the current number of displayed records.

|                                  |                                                                                   |
| -------------------------------- | --------------------------------------------------------------------------------- |
| ![ic_robot](Images/ic_robot.png) | Measurements made by the device in automatic mode.                                |
| ![ic_event](Images/ic_event.png) | Device events - power on/off, reset of dose accumulation, battery discharge, etc. |
| ![ic_rare](Images/ic_rare.png)   | Current parameters of the device - temperature, battery charge, etc.              |

The letter in the upper right corner of the entry indicates that the entry was made in demo mode of the application.

Tapping gear at the top of the screen opens the log display settings. In the settings, you can specify:

<>•What types of measurements to display;
•What types of device events to display;
•Whether to display all records or only those where there was any alarm;
•Whether to display only records with comments (a comment can be set by tapping the corresponding point on the graph of the count rate or dose rate);
•The sort order of records is descending or ascending date.

Tapping the record on the screen displays a dropdown menu:

![LogMenu](Images/logmenu.png)

Show on chart: Display the area corresponding to the selected record on the graph.

Show on map: If the selected record is an automatic measurement or an alarm event and it has location information, then open on the map [pseudo track](pseudo_tracks.htm).

Edit comment: Set a comment for the selected record. The text of the comment is displayed in the log in white on a blue background. Vertical white lines are drawn on graphs for records with comments if the records are of the "Automatic measurement" type.

The “Delete records in interval...“ item makes it possible to select a time interval for deleting records.

Export csv...: Share log file in Excel csv text format. You will be prompted to select the time interval for exporting records and the name of the csv file to export. Only the records that meet the conditions of the filters selected in the log settings, i.e. those that appear in the list, are exported.

Fields in a csv file are separated by semicolons. The values in the "Time stamp" field are decimal 64-bit numbers that represent time in Windows FILETIME format, i.e. the number of 100-nanosecond intervals since January 1, 1601. The time in the "Time stamp" and "Time" fields is local. Values in the "Dose accumulation time, sec." field is the dose accumulation time after the last reset, in seconds.
