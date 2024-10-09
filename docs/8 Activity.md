
The “Activity” tab is designed to determine the absolute and specific activity of the Cs-137 isotope in various loose and watery materials (primarily in food) and the absolute activity of Cs-137 point sources. This isotope is one of the main pollutants after nuclear accidents and tests.

![Activity](Images/activity.png)

**Measurement parameters**

The upper part of the tab displays the parameters that shall be specified before starting the measurement:


| Parameter name | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Geometry       | The parameter is selected from the list and determines the geometry of the sample in which the activity of Cs-137 is evaluated.  <br>If the sample dimensions are small (less than 5 mm), then the geometry should be selected “Point source 5 cm”. In this case, during the measurement, the sample is located at a distance of 5 cm from the “+” symbol on the back cover of the device and from the side of this symbol.<br><br>If the sample is large enough (does not fit the description of the point source above), then one of the containers in the list should be selected. Containers are not included in the device delivery set and should be purchased separately. |
| Product        | Name of the sample material, selected from the list. The parameter if not entered if geometry is selected “Point source 5 cm”.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Weight         | Numerical value of the sample weight in grams with an accuracy of 0.1 g. The parameter is omitted if "Point source 5cm" geometry is selected.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Spectrum       | Displays the spectrum name of the sample taken from the spectrum library, or “Current”if a new spectrum is being accumulated during the measurement process.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Backgroun d    | Name of the background spectrum from the spectra library                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |


**Measurement results**

The results are displayed below the measurement parameters and grouped into: Activity/Specific, MDA/Specific and MPC.

| Result name       | Description                                                                                                                                                                                                                                                                                                                                  |
| ----------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Activity          | Absolute activity of the sample minus the background, in becquerels.                                                                                                                                                                                                                                                                         |
| Specific activity | Specific activity of the sample, based on the injected mass, in becquerels per kilogram. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                                                                        |
| %                 | Estimation of the random error of the current values ​​of absolute and specific activity. The error decreases with increasing the measurement time. At error values ​​greater than 30%, the measured activity values ​​are considered unreliable and are displayed in gray. If it is impossible to estimate the error, dashes are displayed. |
| MDA               | Estimate of the minimum detectable activity, in becquerels. Calculated from the background spectrum and the sample spectrum, taking into account their random errors.                                                                                                                                                                        |
| Specific MDA      | Estimate of the minimum detectable specific activity calculated based on the MDA and the sample mass, in becquerels per kilogram. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                               |
| MPC               | Exceeding the MPC level, in times. MPC is maximum permissible concentration, tabular values ​​are taken for Russia. The parameter is not calculated if geometry is selected “Point source 5 cm”.                                                                                                                                             |

**Spectrum**

At the bottom of the “Activity” tab there is an area for displaying the histogram of the spectrum section, according to which the above estimates are calculated. In the center of the histogram, there is a region of the spectrum where the presence of a Cs-137 peak with an energy of 662 keV is assumed. The region with energies of 662 ±100 keV is displayed in brighter colors. The criterion for the availability of cesium in the sample is the bell-shaped peak on the spectrum, which stands out above the background level, with a maximum in the middle of the graph. If such peak is not visible, then the measured values ​​may be unreliable.

**Start/stop button** (combined) serves to start/stop the measurement. When starting a measurement, you can either continue the current measurement (if any) or start a new one. During the measurement, the current data is saved once a minute, the measurement will automatically continue after reconnecting the device and after restarting the application.

**“Diskette” button** serves to save the obtained spectrum to the spectra library.

**“i” button** serves to display extended information about the measurement.

**"Gear" button** opens the activity measurement settings dialog:

**Activity measuring units:** Becquerel - defined as the activity of a source in which an average of one radioactive decay occurs per second. 1 [Bc] = 1 decay/sec.
Curie is an outdated measure of activity. It is defined as the activity of 1 gram of radium-226 together with daughter radionuclides. 1 [Ci] = 37,000,000,000 Bq.

**Use MPC standards for the country:** select the country for which the MPC standards apply. When you select a country, the list of products available for measuring their activity also changes.

**Offer to save the spectrum when stopping the activity measurement:** If the [activity measurement](activity.htm) is performed in several steps, this option can be disabled so that the application does not offer to save the accumulated spectrum each time the measurement is stopped.

**Measurement procedure**

Use the following methods to assess the sample activity:
[Measurement of sample activity in a container](container.htm)
[Point source activity measurement](point_source.htm)

# 8.1 Measurement of sample activity in a container

Measurement procedure

>[!note]
>IMPORTANT: To determine the activity of loose and watery materials, it is necessary to give them a standard shape by placing them in a special container (containers are not included in the device delivery set and are purchased separately). At the moment, the program calculates activity, when using multiple containers:

|                                                                    |                                                                        |                                                        |                                                |
| ------------------------------------------------------------------ | ---------------------------------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------- |
| ![Marinelli](Images/marinelli.png)             | ![MarinelliRC](Images/marinellirc.png)             | ![Container](Images/container.png) | ![100ml](Images/100ml.png) |
| 0.5 l Marinelli container                                          | 0.5 l Marinelli container                                              | 60 ml container                                        | 100 ml container                               |
|                                                                    |                                                                        |                                                        |                                                |
| ![MarinelliAuthor](Images/marinelliauthor.png) | ![MarinelliAuthor02](Images/marinelliauthor02.png) |                                                        |                                                |
| 0.5 l Marinelli author                                             | 0.2 l Marinelli author                                                 |                                                        |                                                |

You can download the files for 3D printing of the author's containers [here](https://www.thingiverse.com/dnpro/collections/41928551/things).

To measure the mass of the container and sample a balance with an accuracy of at least 1 g will also be required.

1) Charge the device to at least 50% capacity and using the [“Spectrum” mode](spectrum.htm) generate a background spectrum set. When obtaining the spectrum, the device shall always be in the same place where the activity measurement will be carried out. To improve the measurement accuracy, it is recommended to obtain spectra for at least 8 hours, and if possible - a day or more. Save the acquired spectrum to the [spectra library](background.htm) with the name “Background Date/Location” or similar.

2) Open the “Activity” tab of the application and in the dropdown list of the “Geometry:” line select the container used.

3) In the dropdown list of the “Product:” line select the product type.

4) In the “Weight:” line enter the weight (net) of the sample. For this:

•measure the weight of the empty container with the lid;

•fill the container with the sample to capacity, having previously crushed, dried or pressed the sample;

•close the lid and measure the mass of the container with the sample;

•calculate the mass of the sample by the difference between the obtained values, and enter the result in the “Weight:” line (the program allows entering a value with an accuracy of 0.1 g).

5) In the “Background:” line select the previously obtained background spectrum.

6) Place the turned on device on the sample.

•If a 60 ml container is used, place it on a horizontal surface with the lid up. Place the device on the container so that the “+” sign of the back cover of the dosimeter is located strictly above the center of the container lid. In this case, the other side of the device shall rest on some object of the same height as the container (for example, a second container of the same size).

•If a Marinelli container is used, then place the device in the open cavity of the container with the USB connector facing out and the “+” sign inward.

7) At the bottom of the “Activity” tab, in the spectrum histogram display area, click the button with the triangle icon to start the measurement.

8) Perform measurements until the values ​​of the minimum detectable activity (MDA), as well as the measurement error, reach the values ​​that suit you.

# 8.2 Point source activity measurement


Measurement procedure

1) Charge the device to at least 50% capacity and using the “Spectrum” mode generate a background spectrum set. When obtaining the spectrum, the device shall always be in the same place where the activity measurement will be carried out. To improve the measurement accuracy, it is recommended to obtain spectra for at least 8 hours, and if possible - a day or more. Save the acquired spectrum to the spectra library with the name “Background Date/Location” or similar.

2) Open the “Activity” tab of the application and in the dropdown list of the “Geometry:” select “Point source 5 cm”.

3. In the “Background:” line select the previously obtained background spectrum.
    
4. Place the turned on device and the source at a distance from each other so that:
    - ·  the “+” sign of the rear cover of the device was turned towards the source;
    - ·  the geometric center of the source was located on the same line with the “+” sign, perpendicular to the rear cover of the device;
    - ·  the distance to the source, measured from its geometric center to the geometric center of the scintillator, was 5 cm (projections of the scintillator center on the side surfaces of the device are marked with marks, and the projection on the back cover is marked with a “+” sign).
5. At the bottom of the “Activity” tab, in the spectrum histogram display area, click the button with the triangle icon to start the measurement.
6) Perform measurements until the values ?of the minimum detectable activity (MDA), as well as the measurement error, reach the values t?hat suit you.
