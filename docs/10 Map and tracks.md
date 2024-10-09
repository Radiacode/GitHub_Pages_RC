Application RadiaCode equipped with functions of displaying the emission situation on a map in real time, as well as functions of recording routes (“tracks”) and their subsequent download for view.

To access the map, select the “Map” item in the main menu, which is called by tapping the icon ![_NavMenu](Attachments/_navmenu%203.png)top left. To record tracks, the app needs access to the location of the device. Also, the location function of the phone/tablet must be enabled.

![Map](Images/map.png)

|                                                                |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![ic_settings](Attachments/ic_settings%203.png)  | Opens [the settings related to the map](map_settings.htm).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ![ic_route](Attachments/ic_route%201.png)        | Opens [track library](libs.htm).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ![ic_cur_location](Images/ic_cur_location.png)   | Displays a point in the center of the map that corresponds to your current location. A long tap on this icon additionally sets some average map scale.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ![ic_roundgray_wb](Images/ic_roundgray_wb.png)   | Starts or continues recording a track.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ![ic_map_dose_rate](Images/ic_map_dose_rate.png) | Indicates that marker colors are determined from dose rate values. When clicked, switches to the mode of marker coloring by count rate, and the icon on the button is replaced by this: ![ic_map_count_rate](Images/ic_map_count_rate.png) This icon indicates that marker colors are determined by count rate values, and clicking on it switches to the mode of marker coloring by dose rate.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ![ic_more_vert](Images/ic_more_vert.png)         | Opens the drop-down menu:•<br>**Mark:** Enter marker flagging mode. In this mode, tapping a marker flags it for later deletion. The flagged markers are white and surrounded by a pink circle.<br>**•Delete selected...:** After confirmation, delete the flagged markers from the track. Markers are permanently deleted and cannot be recovered.<br>**•Navigate to...:** Opens the drop-down menu:<br>**Maximum/minimum value:** Display on the screen the section of the track on which the marker with the maximum/minimum value (dose rate/count rate) is located.<br>**Start/End of track:** Display the start/end section of the track on the screen.<br>**▪Fit the track on screen:** Automatically select the scale and position of the map so that the entire track fits on the screen.<br>**•Share track:** Export the track data and "share" this file, i.e. save it in smartphone memory, send it by mail or via messenger. For more information, see "[Export and Import](export_import.htm)".<br>**•Track Information:** Open a dialog with detailed information about the track.<br>**•Track picture...:** A drop-down menu opens to control the [image](camera.htm) attached to the track.\| |
| ![ic_a](Images/ic_a.png)                         | Automatically colors markers on the map in accordance with the minimum and maximum dose rate/count rate values. A long tap additionally automatically sets the minimum and maximum values of the displayed markers.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ![_Scale](Images/_scale.png)                     | Expands/hides the color bar graph.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |

**Tracks**

When you record a track, each current location is marked with a circle on the map. The color of the circle corresponds to the emission level or count rate measured at this point, taking into account the color settings on the color scale.

![Track](Images/track.png)

The colors of the markers are determined by the dose rate values or, starting with application version 1.30.00, by the count rate values. The display mode is selected using the corresponding button on the toolbar. Tracks recorded with older versions of the software do not contain count rate information, so marker colors will appear the same in both modes. Tracks recorded by a device whose firmware did not yet support energy compensation essentially contain dose rate values that are directly proportional to the count rate.

To start recording a track, tap the icon ![ic_roundgray_wb](Images/ic_roundgray_wb.png) at the top left of the screen. You will be prompted to enter a track title. After that, recording will start, and the name of the track will be displayed at the top of the screen under the buttons:

![_Recording](Images/_recording.png)

New points appear on the map, and, accordingly, are remembered in the track only when the location changes. In [the application settings,](settings.htm) you can set the minimum position accuracy. It should be borne in mind that the correctness of determining the location depends on many factors - the quality of the phone's GPS module, the interference situation, etc. In the absence of information from the GPS sensor, the smartphone can determine the location using other sources - cell towers and Wi-Fi networks.

When first displayed on the map in the dose rate mode, the marker is colored according to the current value of the dose rate transmitted by the device, and surrounded by a thick gray line. The operational value of the dose rate transmitted by the device lags behind the current calendar moment in time. The lag time depends on the rate of change in the radiation situation: with small changes in dose rate values, the lag can be tens of seconds; with sharp changes, the lag is reduced. As data arrives from the device, operational markers corresponding to the calendar time of the received values ​​are repainted in accordance with the accepted value and acquire the status of permanent ones, the thick stroke disappears. You can turn off the thick outline of operational markers in the map settings. Hot markers are not stored in the database.

Track recording continues until it is explicitly stopped and as long as the application is in communication with the device. When the device is reconnected, track recording resumes automatically.

It should be borne in mind that in the track recording mode, the smartphone consumes a lot of energy and its battery will drain faster. If you do not need to, do not set too small a value for the positioning accuracy in the application settings.

If you tap any circle (marker), information corresponding to this point will be displayed - date/time, measured emission level, count rate, and positioning accuracy:

![_MarkerInfo](Images/_markerinfo.png)

Touching the information window opens a drop-down menu - with its help you can attach a [picture](camera.htm) to the point, remove the point from the track, or simply close the information window.

**Color scale**

The color scale is a quick way to color the track points so that they clearly reflect the changing emission situation. By moving the scale sliders, you can set the minimum dose rate or count rate value, which corresponds to the violet color, and the maximum value, which corresponds to the red one:

![MapScale](Images/mapscale.png)

This example shows that the entire range of measured values ​​is approximately 40...77 μR/h. The purple slider is set to 40.5 μR/h, so all points with the same and lower dose rate level will be purple. The red slider is set to 77.2 μR/h, and all points with the same or higher level will be red. All points between 40 and 77 μR/h will have intermediate colors, from violet to red. In the map settings, you can select a palette of colors to display markers.

In the map settings, you can turn on the function of automatic coloring of markers in accordance with the current maximum and maximum measured value.

Attaching images to track points

In addition to the entire track, it is possible to attach images to individual track points. Attached images are displayed with a camera symbol:

![_PicsOnMap](Images/_picsonmap.png)

There are two ways to attach a picture to a point on a track:

•Take a photo with the [camera](camera.htm). The picture will be attached to the very last point of the track.
•Tap a point on the map. A drop-down menu will open, allowing you to attach a picture to the point.

Tapping the camera icon opens a drop-down menu for image manipulation.

See also:

[Map settings](map_settings.htm)

[Track library](libs.htm)

[Pseudo tracks](pseudo_tracks.htm)

# 10.1 Map settings
To open the map settings, tap ![ic_settings](Attachments/ic_settings%202.png) at the top left of the screen.

Maps API:

It is possible to choose the software platform that provides the maps and their rendering. The default is Google Maps. As an alternative map API you can choose the OpenStreetMap platform ([https://www.openstreetmap.org/)](https://www.openstreetmap.org/)). OpenStreetMap is an open source project with the ability for users to add their own objects to the map.

Google Maps provides an opportunity to choose between the type of map - scheme, satellite photo or hybrid version and works only in online mode, ie, when displayed sections of the map are downloaded by the application from the Google server.

OpenStreetMap displays the map only as a diagram. You can choose between the online mode, when the map is downloaded as raster images-tiles from the servers of OpenStreetMap partner companies, and the offline mode, when preloaded files with vector maps are used for display (see below for details). OpenStreetMap draws markers much faster than Google Maps, so for very large tracks it is more convenient to use it.

Google Maps and OpenStreetMap settings are slightly different. The different settings are listed at [the end of the page](map_settings.htm#osmsettings).

Store location in the database:

Never: The coordinates of your smartphone's current location are not recorded in the database (log).

Only when recording a track: The coordinates of your smartphone's current location are only entered into the database during track recording. This allows you to partially recover a track from the base log as [a pseudo track](pseudo_tracks.htm).

Always: If enabled, the location is entered into the database along with the rest of the information. In the future, you can open on the map [pseudo track](pseudo_tracks.htm) and see the change in the radiation situation associated with the selected location. You should not enable this option unnecessarily, because location determination makes the smartphone consume a lot of power.

Coordinates are stored in the database only if location detection in the smartphone is enabled by the user. Android apps do not have the ability to turn location detection on and off on their own.

Location:

Location resolution and distance between markers on the map: If the location of the smartphone changes by more than the specified number of meters from the previous one, then in [track](map.htm) a new point is recorded. Do not set too low values, since at the same time, the GPS module of the smartphone will work more intensively, while the number of track points will increase rapidly and the rendering of the track on the map will be slower.

Ignore a location if its measurement accuracy is worse than: If the accuracy of the position measurement is worse (greater than) the specified value, the application will ignore the system message about the position change. For example, if you specify to ignore locations with a measurement accuracy worse than 20 meters, and the system reports that the location has changed, but the measurement accuracy is ± 22 meters, then this location change will be ignored.

Ignore location if the distance to the previous point is less than: If the distance between the previous point and the current point is less than the specified value, the application will ignore the system message about the location change. The combination of the last two options allows you to eliminate situations where the system reports small changes in geolocation coordinates measured with poor accuracy.

In a group “Markers” you can choose how the circle markers will be displayed on the map:

- Minimum and maximum dose rate valuefor the marker defines the range of values ​​of the measured dose rate level displayed on the map. Points with a dose rate level outside the specified range are not displayed.

- Automatically shift the minimum and maximum values: if the marker added to the track has a dose rate value that exceeds the boundaries of the levels displayed on the map ("Minimum and maximum dose rate value for the marker"), then change the corresponding boundary so that the marker is visible. For example, if the maximum limit is set to 120 μR/h, and the dose rate of the next marker is 140 μR/h, the maximum displayed value will become 140 μR/h.

- Display markers where the dose rate value is out of bounds defined by color scale: If this option is disabled, then only those points with the dose rate level between the values ​​defined by the sliders will be displayed on the map. Points with values ​​below the purple slider (for example, less than 40.5 μR/h) and above red (77.2 μR/h) will not be displayed.

- Connect markers with a line: Draw a dashed line connecting the markers. This helps to display the intended trajectory of movement if the markers are far apart, but slows down rendering.

- Automatically set marker colors by min./max. dose rate values: Set (including during the track recording process) colors so that purple corresponds to the minimum dose rate in the track, and red - to the maximum value. The triangles on the color bar will be set to their respective positions. If you move one of the triangles, then this option is disabled. It should also be borne in mind that the automatic coloring of markers with a significant number of points slows down the application.

- Enable the auto-coloring option when loading a new track: If auto-coloring was disabled, for example, due to manual manipulations with the color scale, then auto-coloring will be automatically enabled when loading another track or starting recording a new one.

- Disable live data marker stroke: Do not stroke live markers (for which the dose rate value has not yet been transmitted by the device) with a thick gray line.

- Marker size: you can select the diameter of the circles.

- Markers stroke: Marker circles are outlined with a semi-transparent gray line, which allows you to visually perceive them as a set of circles, and not as a solid line if the markers partially overlap. At small map scales, the stroke masks the colors of the circles, so you can turn off the stroke or choose to turn it off automatically at small scales. The track is rendered slightly faster when the stroke is off.

- Decimation of markers: One can choose an additional criterion, taking into account which the markers are decimated when they are added to the map in order to speed up the rendering of large tracks. When adding a new marker, the application compares its parameters with the parameters of the previously added marker. The next marker is NOT added if the following conditions are simultaneously met: 1). The distance between this marker and the previous one is less than specified in the selected criterion (1/4 of the marker radius, 1/2 of the radius, or whole radius). 2). The difference in the dose rate of this marker and the previous one does not exceed 10% of the value of the dose rate of the previous marker.

Decimation of markers affects only their display on the map. This setting does not affect the process of recording a track; non-displayed markers are not deleted from the track.

- Marker palette: you can select the palette of colors that are used to draw the markers.

- Map Auto-Centering: If in the process of recording a track you move the map to the side (for example, to view some other part of the map), then after the specified time the map will display in the center the position corresponding to the current location.

- Track length calculation/Ignore location if its measurement accuracy is worse than: When calculating the track length, do not take into account points for which the accuracy of location determination is worse than specified. This allows for more accurate calculation of the track length.

- "Record" button action: You can select the action to be performed when you touch the "Record" button on the map window toolbar.

- When loading a track: You can choose what to display when opening a track on the map: the beginning of the track, its end, or automatically select the scale and position of the map so that the entire track fits on the screen.

- Display location accuracy: Display in the upper left corner of the map information about the accuracy with which the last location was determined. This function works only if track recording is on. If the location was recorded in the track, then the color of the text in the window will be black, otherwise it will be red (the conditions for recording coordinates are not met).

- Display track length: Display track length information in the upper left corner of the map.

- Display movement speed: Show speed in the upper left corner of the map. This information is provided by the system, the application does not calculate speed and displays it as is. Speed information may be unreliable due to, for example, low accuracy of location determination.

- Show movement direction: Show direction of travel in the upper left corner of the map. This information is provided by the system. By default, direction is designated by one or two letters: N - north, SE - southeast, etc. If you select "Detailed direction (3 letters)" below, the direction will be encoded by one, two or three letters: N - north, SE - southeast, WNW - west-northwest, etc.

- Keep smartphone screen on when map is active: The smartphone screen will not turn off if a map is displayed on the screen.

Some of the settings related to location are found in [the application settings,](settings.htm).

You can import a track with the button ![ic_import](Images/ic_import.png). The system file picker opens.

Export settings (“Share”)

Application RadiaCode can export a track in several formats:

•in its own rctrk format, which is a text format and can be imported back into an application on another smartphone.

•in json format, which is compatible with the export/import format of the Radio Code app for iOS. json files have the same .rctrk extension as native rctrk format files.

•in gpx format (a free text format for storing and exchanging GPS data). gpx files can be opened in a browser with a variety of viewing tools. When exporting the gpx file, the application specifies the dose rate value in micro-roentgen as the altitude above sea level.

•in kmz format (compressed .kml) for viewing in Google Earth ([https://earth.google.com/](https://earth.google.com/)) and in other programs that support the .kml/.kmz format.

When exporting a track in the .kmz format, one can set the following settings:

- Marker size: By default, Google Earth draws markers of some automatically selected size. This setting allows controlling the marker size in Google Earth.

- Marker transparency: One can choose the degree of transparency of the markers: 0% - opaque, 75% - almost transparent.

- Decimation of markers: Do not add a marker to the file if the distance in meters between it and the previous marker is less than the specified one, and the difference in dose rate values ​​is not too large. This allows reducing the number of markers on the map. For decimation, the same algorithms are used as when drawing a track in the application.

- HTML in point descriptions: Each point is assigned a text string that is displayed in Google Earth when the marker is clicked - date/time, dose rate, location accuracy. Google Earth allows using an HTML markup in descriptions, which makes the text more readable. However, not all programs that work with the .kmz format understand HTML correctly, and for such programs, you can turn off HTML in the text.

Settings specific to Google Maps:

In field “Map type” you can choose how the map will look - a diagram, a satellite photo or a hybrid version.

Theme for Diagramthe "Scheme" mode: you can select a map theme: light (the default), dark or let the app select the theme according to the smartphone's light sensor. In the latter case, the theme switches automatically if the light level has changed and remains stable for 10 seconds. Due to the use of the ambient light sensor, the power consumption of the application may increase slightly.

Do not add markers to the map outside of the displayed area: This option can optimize the map performance when there are a lot of points in the track. If the number of points is more than 500, then when moving and scaling the map, all markers are deleted and only those that are within the map area visible on the screen are re-added. This causes track markers to blink, but the map is drawn faster due to the limited number of markers added. The effectiveness of this technology depends on the ratio of visible markers and their total number in the track (if the entire track is displayed on the map, then the efficiency will even be negative), as well as the speed of the smartphone.

Settings specific to OpenStreetMap:

OpenStreetMap map source: by default (online), the variant when the map is loaded as ready raster images-tiles from the servers of companies-partners of OpenStreetMap is applied. The second option is to work with maps in offline mode, i.e., no Internet connection is required for this. The source of maps are vector map files, which you need to download yourself from one of the sites listed on the page [https://download.mapsforge.org/](https://download.mapsforge.org/) (it's more convenient to do it with a computer) and put it in the RadiaCode app folder on your smartphone named /sdcard/Android/data/com.almacode.radiacode/files/Maps.

When downloading maps, it is better to choose the format of version 5, maps of this format are in the folder with the name v5:

![Mapsforge](Images/mapsforge.png)

At the moment Mapsforge library does not support work with files given the restrictions on access to files that impose the rules of Android system versions 11+, so the map files must be placed in the folder whose name is given above.

In offline mode, map rendering, i.e. the conversion of vector information into a picture, is performed by the Mapsforge library, which is built into the application. This operation requires some smartphone processor resources. When you move the map around the screen and zoom in, the app will consume more power than in online mode.

Map theme: In offline mode, you can choose between two display options, which differ mainly in color palette.

Image scaling: In online mode, the application obtains images of areas of the map with a low resolution. On high-resolution smartphone screens, the inscriptions on such a map look too small, so the images have to be scaled. After scaling, the final image may look a little blurry, but you have to choose between image quality and inscription size. You can find the optimal ratio by using manual scaling. Offline mode does not have this problem, but you can still experiment with the scale.

**Marker rendering optimization:** In offline mode, you can select the way that the OpenStreetMap library will use to optimize marker rendering. If large tracks take too long to render, you can try changing this setting.

# 10.2 Track library

The list of saved tracks is displayed. For each track, you can see its name, which was set when you saved it, the date when you started recording, the time spent on the way, the number of points in the track and the total length of the track in kilometers. For tracks that were created by a device with firmware that does not support energy compensation, a yellow icon is displayed in the lower right corner.

It is possible to create folders for more convenient organization of the library. You can manage folders through the options menu, which is accessed by tapping the three-dot icon in the top right corner of the screen. The options menu also contains:

- **Search:** An input line appears where you can enter part of the track name. Only track names containing the entered substring will remain on the screen. The search is performed within the displayed folder, i.e. this function essentially works as a filter. To find a track located in a folder, you need to switch the display to "Simple list without folders" mode through the same options menu before searching.
- **Track import:** The system .rctrk file picker opens. You can import a file that was previously exported by an application into the library RadiaCode on the smartphone.

    Tapping a line opens a dropdown menu:
    
- **Open track on the map:** Load a track to view.
-  **Share a track:** Export the track data to a text file and "share" this file, i.e. save it in smartphone memory, send it by mail or via messenger. The file format can be selected in the map settings.
- **Rename track:** Set a new name for the track.
- **Edit comment:** Set or edit a comment for the track. A comment is an arbitrary text that is displayed for the track in the library in blue.
- **Delete track:** Remove track data from the library.
- **Move to folder:** Move track to another folder
- **Mark:** Switch to the track marking mode. A check mark appears at the bottom left of the graph:
![[Images/_spg_mark.png]]

. Select by tapping all tracks, with which the group operation will be performed, and tap the symbol with three vertical dots in the upper right corner of the screen: 
![[_trk_options.png]]

A dropdown menu will appear:

- ·  Select all: Mark all tracks in the library.
- ·  Invert selection: Make unmarked tracks marked and marked ones unmarked.
- ·  Delete selected: Delete marked tracks after confirmation.
- ·  Export selected: "Share" all the selected tracks. For the marked tracks, files are generated in the format selected in the settings - rctrk, gpx or kmz. These files are then compressed and exported as a zip archive. If folders are selected, all tracks from the selected folders, including nested ones, are also exported. It is also possible to export all the tracks contained in the folder without marking it - the "Export folder" command is available in the menu that appears when you long-tap the folder.
- ·  Move to folder: Move the selected tracks and/or folders to another folder.
- ·  “Cancel”: Unselect all tracks and exit the mode. The same is done with the “Back” button on the smartphone.  
    Tapping the plus icon allows you to add a new track and start recording it.
# 10.3 Pseudo tracks

A pseudo track is a track generated by the application based on the dose rate data that was written to the database when the option is enabled “[Save geographic coordinates of measurements in the database](map_settings.htm)”.

To build a pseudo-track, select the desired point on the graph or the desired entry in the [log](log.htm) and make a long tap on the screen. A dropdown menu will open. Select the “Show on the map” item in it (it will be available only if the above option was enabled during the measurement and the application received location data from the system). You will be prompted to select time limits for creating a pseudo track:

![_PseudoTrack](Images/_pseudotrack.png)

The map will open, it will display the markers that fall within the selected time interval. It should be taken into account that not operational, but already processed data are entered into the database, which come from the device with a frequency that depends on the current radiation situation. For small changes in dose rate values, data is received at a frequency of approximately 2 minutes, with sharp changes, data is received more frequently. When creating a pseudo track, all map settings are taken into account and the same decimation and filtering algorithms are applied as when building a regular track.

The pseudo track displayed on the map can be saved in the tracks library using the button on the toolbar:

![_SavePseudoTrack](Images/_savepseudotrack.png)