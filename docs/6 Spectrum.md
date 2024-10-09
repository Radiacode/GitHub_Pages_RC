This window displays the energy spectrum of the photon (gamma and X-ray) radiation, typed by the device over a certain period of time. When you connect the device to the smartphone, the app reads the spectrum data from the device. Subsequently, the spectrum graph is updated either automatically at the interval specified in the settings, or manually.

![Spectrum](Images/spectrum.png)

At the top right of the graph you can see:

•the time for which the spectrum data was accumulated, in the format HH:MM:SS.
•The average pulse count rate, i.e. the sum of the number of pulses for all channels, divided by the time of data accumulation.
•Average dose rate of X-ray and gamma radiation over the time of spectrum accumulation.
•X-ray and gamma radiation dose over the accumulation time of the spectrum.
•The way the graph is updated, or, for [the "View Spectrum" window](spectrum_view.htm), the name of the spectrum.

In the mode of displaying the graph of difference between spectrum and background the values of count rate and dose rate will be equal to the difference of these values for spectrum and background. The accumulated dose will be calculated by the formula (Ds - Db) * Ts, where Ds is the spectrum dose, Db is the background dose, Ts is the spectrum accumulation time. In difference mode, spectrum information is displayed in italics as a reminder.

The display of each item except the last is controlled by the corresponding setting. Unnecessary data can be turned off to save screen space.

The part of the graph in which the shape of the spectrum should be considered unreliable due to the small volume of events accumulated there is drawn in gray.

Depending on the settings, the X-axis can display either channel numbers or photon energy. The Y-axis can display either the number of pulses or the count rate. The Y-axis scale can be linear or logarithmic.

| ![ic_settings](Images/ic_settings.png)       | Opens the [[#Spectrum settings]].                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ---------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lin.                                                       | Select the linear scale of the Y-axis                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| Log.                                                       | Select the logarithmic scale of the Y-axis.\|                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ![ic_sp_refresh](Images/ic_sp_refresh.png)   | Refresh spectrum data. The application reads the current data from the device and updates the graph regardless of the update method selected in the settings (manual or automatic).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ![ic_library](Images/ic_library.png)         | Open [spectra library](background.htm).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ![ic_sp_zoom_in](Images/ic_sp_zoom_in.png)   | Enlarge the graph (zoom in). The graph can be scrolled horizontally. Long press of this button increases the zoom to the maximum. The current scale value is displayed in the lower left corner of the screen                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| ![ic_sp_zoom_out](Images/ic_sp_zoom_out.png) | Zoom out. Long press of this button decreases the scale to one.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ![ic_more_horiz](Images/ic_more_horiz.png)   | Open the dropdown menu. Actions are available in the menu:<br><br>•**Restart accumulation of** spectrum data. Confirmation is requested before restarting.<br><br>•**Share spectrum:** Export spectrum data to a text file with the .csv or .xml extension ([export](share.htm)) and "share" this file, i.e. save it in the smartphone memory, send it by mail or via messenger.<br><br>•**Save spectrum to library:** Save spectrum to database. In the future, the spectrum can be used as a background, shared, etc. If the “Set as current background” option is left enabled in the spectrum saving request window, the saved spectrum is selected as the background to be displayed together with the spectrum. The background name is displayed in the vertical text box along the Y-axis.<br><br>•**Spectrum Information:** A window will open with detailed information about the spectrum, background and the difference between them.<br><br>•**Isotope** info: Show detailed information about the isotope that corresponds to the tapping point on the plot.<br><br>**•Attach the selected isotope:** Plot the lines of the currently displayed isotope or decay chain on the graph. The lines will be displayed in their places when moving the pointer, zooming and flipping the graph, etc., until the lock is explicitly released by the "Unlock selected isotope" menu item.<br><br>**•Detach the selected isotope:** Unlock the isotope or decay chain lines set by the "Attach the selected isotope" command.<br><br>**•Device Calibration:** Perform the [calibration procedure for the energy scale of the device](calibrate.htm).\| |
### Spectrum settings 
The spectrum settings are called by the ![ic_settings](Images/ic_settings.png) button on the "Spectrum" and "View" tabs. The spectrum settings are the same for both pages, but they are independent of each other.

•Scale of the Y-axis - linear or logarithmic. Fast scale switching - with icons “Lin.” and “Log.”.

•Units of the Y-axis - the number of pulses or the count rate.

•X-axis units - channel number or photon energy.

•Graph update: either automatically at a preset interval or manually with the button ![ic_sp_refresh](Images/ic_sp_refresh.png).

•Show last channel: Turn on/off the display of the last channel data. The counter of the last channel includes not only the data of this channel itself, but also all data outside the range displayed on the graph, so it may not always be interesting to look at the last channel.

•Drawing the graph: You can choose to fill the spectrum graph with color (fill) and stroke with a line, or one of these options.

•Drawing the background: You can set the background to fill the graph with a color (fill) and stroke with a line, or one of these options.

•Displaying the background: cm. [Using the background](background.htm).

•Display isotope information: In the application window title bar, display information about the characteristic gamma line of the isotope and decay chain, and display an icon to go to a website for more information. Disabling this option also disables the display of all isotope lines.

❑Display the position of the gamma lines: Draw turquoise clue lines corresponding to the position of isotope energies.

❑Display the intensity of the gamma lines: Draw red clue lines corresponding to the positions and intensities of isotope energies.

❑Draw markers on the lines of intensity: Display the gamma line intensity amplitude as red dots on the isotope lines.

•"Spectrum Information" group: You can select which spectrum information to display in the upper right corner of the graph:

❑ Accumulation time is the total recording time of the spectrum.

❑ The number of pulses is the total number of pulses in the spectrum, for the entire time of its recording.

❑ The count rate is the average value of the count rate of the spectrum over all channels during the accumulation time, i.e. the sum of the number of pulses of all channels divided by the accumulation time.

❑ Dose rate is the average value of the dose rate of the spectrum over the accumulation time. The dose rate is calculated using a special algorithm.

❑ Dose is the radiation dose accumulated during the accumulation of the spectrum.

❑ Hardness is the hardness coefficient of the spectrum calculated from the dose rate and count rate.

•Display "zoom": Select the magnifier display mode. Zoom is a small window in which a section of the graph corresponding to the vertical marker line is visible at an enlarged scale. In the "Automatic" mode, the application itself selects the zoom position according to the vertical marker line position.

•Show the amplification slider: Below the spectrum graph you can see the slider that adjusts the "amplification" of the histogram, see below.

•Show the filter slider: Below the spectrum graph you can see the slider that adjusts the degree of filtering (smoothing) of the histogram, see below.

•Gaps between bars in the “Fill only” mode: Draw bars with gaps between them, rather than a solid graph contour line, if the selected scale allows it and the "Draw a polyline instead of a histogram" option is disabled.

•Draw a polyline instead of a histogram: instead of rectangular bars (histogram), draw a polyline that connects the midpoints of the tops of the bars. The graph is not entirely “true”, because the accumulation of the spectrum is still discrete for each channel. In this mode, the option “Gaps between bars in the “Fill only” mode” has no meaning and is ignored.

•Do not display negative values ​​in the spectrum-background difference mode: Display only the top of the spectrum versus background difference plot that corresponds to positive difference values. Negative values ​​will be displayed as zero.

•Automatically scale the Y-axis: When the scale is more than 1, automatically select the scale of the Y axis in accordance with the maximum value of the data in the displayed area of ​​the graph.

•Export format: Choose in which format [export the spectrum](share.htm).

•csv Export separator: you can specify which symbol to use when exporting the spectrum to a text file with the .csv extension (comma or semicolon).

•Calibration coefficients: a page opens where you can specify the calibration factors a0, a1 and a2.

Spectrum calibration is performed to convert the number of the spectrum channel to the value of the emission energy in keV using a polynomial of the 2nd degree of the form:

E = a0 + a1·x + a2·x2,

where

x is the channel number;

a0, a1, a2 are calibration coefficients.

**Tapping the graph** at a display scale of x1, displays the cursor lines. The vertical line corresponding to the position on the X-axis can be moved by tapping the screen at the desired point or moving your finger across the screen. The horizontal line is automatically positioned to the position of the pointer on the X-axis.

To display marker lines at a scale greater than x1, do long tap on the screen, then marker lines will appear. Move the vertical line left and right without lifting your finger from the screen.

If marker lines are present, then a "magnifying glass" ("zoom") is displayed in the lower corner of the spectrum graph by default - a small window in which a section of the graph corresponding to the vertical marker line is visible at an enlarged scale. The magnifier allows you to position the marker lines on the peaks more precisely. In the [spectrum settings](spectrum_settings.htm), you can set the position of the magnifier on the chart or turn it off.

**Quick double tap** toggles the display mode between linear and logarithmic.

At the bottom of the spectrum window there is a slider that controls “enhancement” of a histogram. A curve of the following type is superimposed on the graph:

![sp_amplifier](Images/sp_amplifier.png)

This allows subtle peaks to appear on the graph. For each channel, the value is calculated by the formula Vn = Vn An F + 1, where:

n - channel number

Vn - spectrum value (number of pulses or count rate) in channel n

An - the value at the corresponding point of the amplifying curve

F - gain factor, which is set by the slider, from 0 to 5.

In amplification mode with F >= 1, the digitization of the Y axis is not displayed.

**Filter Engine** applies a smoothing algorithm to the spectrum graph. The higher the filter value, the more the graph is smoothed.

The spectrum graph is also available as a [widget](widgets.htm).

[Background Usage and Spectra Library](spectrum.htm)

[Displaying isotope information](isotopes.htm)

[Spectrum settings](spectrum_settings.htm)

[View tab](spectrum_view.htm)

[Export and import of spectra](share.htm)

[Calibrating the energy scale of the device](calibrate.htm)
# 6.1 Background Usage and Spectra Library

In the application RadiaCode it is possible to display on the graph not only the spectrum of accumulated emission, but also to compare the spectrum with the previously measured background spectrum. One can display spectrum and background graphs at the same time in the overlay mode, or display a graph of the difference between the values ​​of the current spectrum and the background.

To use a background, you first need to measure this background with the device over a period of time. Then you need to save the resulting spectrum to the spectrum library. To do this, tap the local menu call button in the spectrum window: ![SpectrumLocalMenu](Images/spectrumlocalmenu.png)

Select “Save Spectrum to Library” from the dropdown menu. You will be prompted to name the spectrum. The spectrum will be displayed with this name in the library list. If you leave the “Set as Current Background” option enabled, then after saving the spectrum will be displayed on the graph as a background. You can also select the background from the spectra library in future.

There are two modes for displaying spectrum and background. In the overlay mode, the background graph is drawn on top of the spectrum graph - the spectrum is drawn in orange, the background in green. In the second mode, the difference between the spectrum and the background is displayed, the color of the graph is purple.

In the mode of displaying the difference between the spectrum and the background, the difference in the count rate is displayed, since the background and the current spectrum always have different accumulation times and it makes no sense to subtract the number of accumulated pulses.

>[!warning] If using spectrum and background from different devices for superposition RadiaCode-10X, it should be borne in mind that different devices have different calibration factors. When overlaying spectra graphs, the application compares them per channel (the first channel with the first channel, the second channel with the second channel, etc.). Different devices have different emission energies corresponding to the same spectral channels, therefore, when the graphs from different devices are superimposed, differences in the positions of the peaks corresponding to the same emission energy will appear.

If the application detects such a situation, it issues an appropriate warning. Device RadiaCode-10X is identified by its serial number.
### Spectra library

The spectra, spectrograms and tracks storages are called libraries and are stored in the application database. We will call a spectrum, spectrogram and track by the word "object".

To open a library, tap the ![ic_library](Images/ic_library.png) symbol on the control bar (toolbar) of the "Spectrum", "View" or "Spectrogram" tab. The track library is opened by the ![ic_route](Images/ic_route.png) icon on the map toolbar.

A list of saved objects is displayed. For each object, its name, which was specified when saving, the recording start date, the serial number of the device and other information corresponding to the type of object are displayed.  For tracks that were created by a device with firmware that does not support energy compensation, a yellow icon is displayed in the lower right corner. For [8-bit spectra](sp10bit.htm) created by a device with firmware version less than 4.00, an orange marker with the number 8 is displayed in the lower right corner. For each saved spectrum, its graph in the logarithmic scale, name and accumulation time are displayed.

![SpectrumLib](Images/spectrumlib.png)

It is possible to create [folders](folders.htm) for more convenient organization of the library. You can manage folders through the options menu, which is accessed by tapping the three-dot icon in the top right corner of the screen. The options menu also contains:

•Search: An input line appears where you can enter part of the object name. Only object names containing the entered substring will remain on the screen. The search is performed within the displayed folder, i.e. this function essentially works as a filter. To find a object located in a folder, you need to switch the display to "Simple list without folders" mode through the same options menu before searching.

•Import object: The system file selector opens. For more information, see "[Export and Import](export_import.htm)".

Tapping a line opens a dropdown menu:

•Open object:  Load an object for viewing (the track opens on the map). If the object is a spectrogram and is currently being recorded, it continues in the background. To return to the graph of the spectrogram being recorded, tap the ![ic_more_horiz](Attachments/ic_more_horiz%201.png) button on the "Spectrogram" tab and select "Close spectrogram".

•Share object: Export the object data and "share" this file, i.e. save it in smartphone memory, send it by mail or via messenger. For more information, see "[Export and Import](export_import.htm)".

•Rename object: Set a new name for the object.

•Edit comment: Set or edit a comment for the object. A comment is an arbitrary text that is displayed for the object in the library in blue.

•Delete object: Delete object data from the library.

•Move to folder: [Move](folders.htm) object to another folder.

•Picture: A menu appears to manage the attached [picture](camera.htm).

•Select: Switch to object marking mode. A check mark appears at the bottom left of the graph:
 ![_spg_mark](Images/_spg_mark.png). 
Select by tapping all objects, with which the group operation will be performed, and tap the symbol with three vertical dots in the upper right corner of the screen: ![_spg_more](Images/_spg_more.png)

A dropdown menu will appear:

•Select all: Mark all objects in the library.
•Invert selection: Make unmarked objects marked and marked ones unmarked.
•Delete selected: Delete marked objects after confirmation.
•Export selected: [Export](export_import.htm) all the selected objects.
•Move to folder: [Move](folders.htm) the selected spectra and/or folders to another folder.
•Sorting: Select the sorting mode for objects in the list - by name/date, ascending/descending.
•Cancel: Unselect all objects and exit the mode. The same is done with the “Back” button on the smartphone.

For spectra, there are additional items in the menu:

•Merge selected: Perform the operation of channel-by-channel addition of the data of the selected spectra. Only spectra obtained with the same device can be combined. RadiaCode-10X. A new spectrum is created, you are prompted to enter its name for saving in the spectra library. The number of pulses of each channel of the combined spectrum is the sum of the number of pulses in the corresponding channels of the combined spectra. The accumulation time is calculated in the same way.

•Edit calib. coeffs: A dialog window opens, where you can set the calibration factors for all selected spectra. This can be useful if the device, with which the spectra were taken, was recalibrated.

Additional items in the track library menu, if several are selected:

•Merge Selected: Merge the selected tracks into one. The tracks are merged without any checks. You are prompted to select a name for the merged track and open it on the map.

# 6.2 Displaying isotope information

When you tap the graph and move your finger across the screen, the application header displays information about the radioactive isotope, the energy of which corresponds to the cursor position:

![isotope_title](Images/isotope_title.png)

The name of the isotope, the corresponding energy is displayed, in square brackets - the energy corresponding to the cursor line on the spectrum graph. The name of the decay chain for the isotope is displayed below.

To see examples of spectra of common isotopes, tap [here](https://scan-electronics.com/en/isotopes).

In case the option "Display gamma line position" is enabled:

The pink line marks the position of the isotope energy line. If the isotope has accompanying lines, then they are displayed in turquoise ([see the figure in the “Spectrum” topic](spectrum.htm)). The dotted lines correspond to the X-ray lines.

If there are several isotopes with close energies, then information about that isotope is displayed, the energy line of which is closest to the value of the energy corresponding to the cursor.

If the "Display gamma lines intensity" or "Draw markers on intensity lines" option is enabled, red lines/markers corresponding to the intensity of gamma radiation lines, relative to the activity of the parent nuclide, are drawn over or instead of turquoise isotope lines.

# 6.3 View tab

The “View” tab is intended for static viewing of spectra from [spectra libraries](background.htm). The functionality of the tab and control is the same as on the main “Spectrum” tab, except that the update button is replaced with a button for switching to the spectrum library, and the name of the spectrum is displayed instead of information about the update.

To load a spectrum for viewing, you need to open the spectra library, tap the desired spectrum and select “Load to view” in the dropdown menu.

The preview displays the same background as in the main Spectrum tab.

# 6.3 Export and import of spectra

Spectra are exported with the command “Share”, which is called through the dropdown menus ![ic_more_horiz](Attachments/ic_more_horiz%202.png)in the “Spectrum” and “View” tabs, as well as the window of the spectra library.

Two formats are supported: .xml (default) and .csv. Both formats are supported by the popular Becquerel Monitor software. You can select the export format in the spectrum settings.

A file in xml format can simultaneously include a spectrum and a background and contains all information about them - names, number of channels, spectrum accumulation time, calibration factors and the serial number of the device on which the spectrum and background were taken. This format is self-sufficient and does not require additional steps from the user when importing; xml files can be imported directly from instant messengers like WhatsApp and Telegram.

A csv file is a text file with a .csv extension that can be used not only with the Becquerel monitor, but also with other applications due to the simplicity of its format. Only pairs of values ​​”channel number, number of pulses” are written to the file. In the spectrum settings, you can choose which separator to use - comma or semicolon. The file name is formed as
    > [note](“Spectrum_<Current date/time>_<Accumulation time in seconds>s.csv”, for example, Spectrum_2021-05-12_13-53-55_1426s.csv. )
    
When importing csv file into application RadiaCode a window is displayed where it is proposed to enter the spectrum name, the accumulation time (if it was not possible to determine it from the file name), as well as the serial number of the device, on which the spectrum was taken, and the calibration factors. It is possible to indicate to the application that the imported spectrum was taken with the currently connected device - for this there is a special button “Copy factors and serial number from the device”.

For spectrum and background overlapping from different devices RadiaCode-10X read [here]().

It is also possible to ![export several spectra simultaneously](background.htm) as a zip archive.

Importing a spectrum to the library

Application RadiaCode is registered in the smartphone as a handler for files with the .xml and .csv extensions. When tapping a file with the .xml or .csv extension in any other Android application, for example, in WhatsApp or Telegram, the application RadiaCode will be in the “Open with...” list. If you open the file with RadiaCode, the spectrum will be imported into the spectrum library, you will be prompted to set the import parameters for the spectrum.

You can also import a spectrum using the button ![[Images/ic_import.png]]. The system file picker opens.


# 6.5 Calibrating the energy scale of the device

Calibrating the energy scale of the spectrum is necessary to accurately determine the energy of the gamma lines of the spectrum by the channel number. The devices undergo a calibration process at the factory, but detector parameters may change over time, necessitating a calibration update. It would require sources with known isotopic composition and energies in advance. The calibration points are the vertices of the peaks on the gamma spectrum. The result of the calibration is the values of the calibration factors, which are used by the device to convert the spectrum channel number into the radiation energy value in keV using a polynomial of degree 2 kind:

E = a0 + a1·x + a2·x2,

where

x is the channel number;

a0, a1, a2 are calibration coefficients.

Spectrum energy scale calibration procedure

The calibration is performed at three points, which ensures sufficient linearity over the entire range of energies under study. To perform the calibration, the user will need a spectrum containing mono-energy lines, preferably located at the beginning, middle and end of the energy scale. For example, the following isotopes produce such lines:

•K-40 (1461 keV);

•Am-241 (59 keV);

•Lu-176 (202, 307 keV);

•Cs-137 (32, 662 keV);

•Th-232 (238, 583, 2614 keV);

•Ra-226 (78, 351, 609 keV);

>[!Caution] 
>You are solely responsible for any potential legal consequences and potential health risks associated with the acquisition, storage, and handling of radioactive materials. Please ensure that while working with radioactive materials, you do not violate local laws and regulations, and observe all safety precautions when handling them.

The most convenient and simple for calibration is Th-232, a naturally occurring element. In most countries around the world, small quantities of Th-232 are legal and available for purchase in local stores, for example, in the form of welding electrodes WT-20.

More details are explained in this instructional calibration [video.](https://youtube.com/embed/ZHGLb_jWpuk)

You can also use alternative sources or their combinations for calibration. For example Cs-137 and K-40. It is not necessary to collect the spectrum with both sources at once, you can collect two separate spectra and memorize the channels where the lines are located during calibration. For example, after collecting the spectrum of Cs-137, remember that on channel 3 there was a peak with an energy of 32 keV, and on channel 66 there was a peak with an energy of 662 keV. And after collecting the K-40 spectrum, by selecting these channels, enter the appropriate energy (32, 662, 1461 keV).

For three-point calibration with a single source, it is best to use Th-232-based sources, but a certain peculiarity must be taken into account: the first line is better chosen at the low-energy level, the X-ray fluorescence line. If the source is a thoriated electrode, the X-ray fluorescence energy will be about 65 keV, but if the source does not contain heavy elements, the line will have an energy of about 88 keV.

After calibrating the device, it is desirable to test it on sources with a different isotopic composition. Also, because of the nonlinearity introduced by the discreteness of the channel step, the lines may not always fall exactly into the channel where they are supposed to be. This is especially true at the beginning of the spectrum.

If a rough calibration without a source is necessary, the K-40 isotope is recommended. It is necessary to dial the background spectrum, where the peak at 1461 keV or potassium fertilizer will be clearly visible, and the peak should be completely colored in yellow. Then, entering the settings, change the calibration factor A1 in increments of 0.1 until the top of the peak is at 1461 keV.

**Calibration procedure**

1) Place the device and the reference source to be measured as close as possible to each other. The detector should be placed with a "+" sign on the source or, if the source is powerful, pointed in its direction with a "+" sign. It is desirable that the count rate should not exceed 500 cps during calibration.

2) In the "Spectrum" tab, reset the spectrum by clicking on ![ic_more_horiz](Images/ic_more_horiz.png) and select "Restart Accumulation" from the drop-down menu.

3) Having determined the choice of reference points, wait until all spectral lines (Gaussians), on which the calibration will be carried out, are colored yellow, which will indicate sufficient statistical reliability of the spectrum data.

4) Tap on ![ic_more_horiz](Images/ic_more_horiz.png)and select "Energy Scale Calibration" from the drop-down menu. At the top of the tab, you will be prompted to enter the energy value:

![_calib](Images/_calib.png)

5) Touch the graph and, by moving the marker lines, select the first point on the graph. Enter the energy corresponding to the point next to the "Next" button. Tap the "Next" button.

6) Repeat this manipulation twice and select the "Done" button.

7) The application will check the channel number values for validity. If the values are invalid, a diagnostic message about it will be displayed. If the values are acceptable, a window will be displayed with a table with energy values and corresponding spectrum channel numbers, and under the table the calculated values of the calibration factors:

![_calib_table](Images/_calib_table.png)

Invalid values of calibration factors are displayed in red. The application blocks the ability to write such values to the device.

You can manually correct the table data, and changing energies and/or channel numbers will cause automatic recalculation of the factor values.

8) Tap the "Program factors to device" button to complete the calibration. If the calibration was initiated from the View tab, the button will save the spectrum open for viewing to the library with new coefficients.

If you need to return the factory calibration of the device or correct the calibration factors manually, you can use the "Calibration factors" button in the [“Device settings” dialog box](device_settings.htm)dialog box.

# 6.6 1024 spectrum channels instead of 256

Device firmware version 4+ supports 1024-channel spectra. Earlier firmware versions supported 256-channel spectra.

The number of spectrum channels is determined by the digit capacity of the ADC used, which digitizes the signal of the device's scintillation detector. The higher bit rate, i.e. 10 bits instead of 8 bits, allows 1024 channels of spectrum. This provides a clearer separation of the spectrum peaks in the low energy region of radiation. The transition to 10-bit spectra became possible due to application of special algorithms and techniques of signal processing at the ADC output. These algorithms minimized the effect of the nonlinearity of the ADC characteristic on the shape of the spectrum.

Application RadiaCode works with 10-bit spectra. When loading from the spectra library and importing old 8-bit spectra (256 channels) from files, they are converted to 10-bit spectra (1024 channels). It should be kept in mind that:

•When converting spectra from 8-bit to 10-bit, the values of calibration coefficients are recalculated: the value of a0 does not change, a1 decreases by a factor of 4, a2 decreases by a factor of 16.

•In the spectra and spectrogram library, 8-bit spectra are labeled with an orange circle with the number 8 in the lower right corner. Calibration coefficients are displayed as converted for a 10-bit spectrum.

•The 1024-channel spectra and spectrograms are always stored in the spectra and spectrogram library and exported.

•Drawing and processing of large spectrograms may be slower due to the increased number of channels.

•The application will work normally with a device that has firmware version less than 4.00 that produces 256-channel spectra. However, it is recommended to update the firmware to the latest version.

•Earlier versions of the application designed to work with 256-channel spectra will not work correctly with a device that has firmware version 4+.