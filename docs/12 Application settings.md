Application settings are available through the navigation menu (pictogram ![_NavMenu](Attachments/_navmenu%204.png)in the upper left corner of the screen).

Please note that to save the settings, you need to tap the “OK” button at the bottom of the screen: ![_Ok](Images/_ok.png)

Application language: Tap to select the language of the application interface. The Russian language is available if it is supported by the mobile device.

Groups in the settings dialogs: Settings in dialogs are organized into groups. By default, all groups are collapsed, which gives them a compact appearance. To expand a group, tap it. If you select the "Always Expanded" setting, all settings groups in all dialogs will be displayed in expanded view. If the "Remember State" option is enabled, the application will remember which settings groups have been expanded and expand them the next time you enter the dialog. You can also enable group collapse/expand animation.

A long tap on the triangle in the upper-right corner of the group opens or closes all groups in the dialog.

Measuring unit: Select in which units the information about the recorded radiation level is displayed: Roentgens (R), Sieverts (Sv) or Biological Rad Equivalent (rem). Rem is an obsolete unit of measurement of equivalent dose of ionizing radiation in the GHS system.

Count rate units: You can choose to display the count rate in pulses per second or pulses per minute (pulses per second multiplied by 60). The setting affects the entire application, including the spectrum.

Min. dose units of dose in Sievert: By default, the dose and dose rate are displayed in units that are automatically selected by the program: pico-, nano-, micro-, etc. If the unit of measurement in the device settings is set to Sieverts, this option allows you to select microSieverts as the minimum scale, as shown on the device display. Temperature Units: You can select whether the device temperature is displayed in Celsius or Fahrenheit.

Units of temperature: You can choose whether to display the device temperature in Celsius or Fahrenheit.

Distance units: You can choose in which units the distance for tracks will be displayed - in kilometers or in miles (1 mile = 1.609344 km).

Duplicate alarm sounds and device vibration on the phone: When an alarm occurs, the smartphone will beep and vibrate in parallel with the device.

Sound indication of the counting speed (clicks): Issue sound of clicks with a frequency proportional to the count rate. To generate clicks, operational information about the count rate is used, which is issued by the device. You can select the volume of clicks and the type of click sound. The "Mute click sounds on calls" option forces the application to make an attempt to track incoming and outgoing smartphone calls, including messenger calls.

Phone signals: You can select the volume of the alarm sounds that your smartphone emits. Actual volume level depends on smartphone model and settings.

Connect/disconnect sounds: Give a signal when the connection between the control panel and the application is established or lost. You can set the volume of these signals. If the connection with the device is lost, the application tries to reconnect with it with an interval of about 30 seconds.

Push notification when communication with the device is lost: Provide a pop-up notification when communication with the device is lost. When the connection is re-established, the notification disappears.

Push notifications for alarms: You can instruct the application to issue pop-up notifications when device alarms occur, either always, or only when the application window is inactive. Pop-up notifications are issued regardless of whether the alarm sounds of the device are turned on or off and can be useful, among other things, for indicating alarms on any kind of Smart-watch connected to a smartphone. In order for push notifications to appear, they should be enabled for the application RadiaCode in the “Application” settings of the smartphone.

Device battery: You can tell the application to issue push notifications if the battery charge level of the device becomes less than the specified value, when the battery is fully charged, as well as in the case when the device itself turns off its power due to a complete battery discharge. A notification about a decrease in the charge level is issued once and does not repeat until the application is restarted or until the device's battery charge again drops from a higher value to the specified threshold.

Tab titles: Choose how to display the tab titles on the application screen - as text ("Home", "Journal", "Spectrum", ...) or as icons. When displayed as icons, icons of all the tabs always fit on the screen.

Start page: You can select which page (tab) will be active when the application starts. If the "Open map" option is set, the map will be opened after activating the page.

Widgets: You can set the background transparency for the application widgets, and separately - the transparency of the text and graphs displayed in the widgets. Widgets are opaque by default.

Screen orientation: You can select one of the options to lock the smartphone screen in a preset position when the application is active.

Database Backups: Automatically create database backups when the application starts. You can choose how often to create backups and how many copies to keep. Backup copies of the database file are created in the Backup subfolder of the application's working folder and have names in the YYYY-MM-DD.db format, for example, 2023-12-08.db. The "Restore backup..." button displays a list of copies available for recovery. When restoring, the application is restarted.

Use more colors in the interface: In some elements of the application interface, use other colors instead of white to improve readability. This applies mainly to the spectrum and track libraries.

Do not turn off the smartphone screen when the application is active: The smartphone screen will not turn off if an app is displayed on the screen RadiaCode.

An animation of the icon in the status bar when the device is connected: If this option is enabled, the app has established a connection with the device, and the app is inactive, the app icon in the smartphone status bar will change appearance every few seconds. This allows you to see if the device is connected to the app without activating the app.
<p id="d_mode">Diagnostic Mode- enable extended information output to the application log file. When a crash occurs, the extended log can help developers figure out the cause of the crash.</p>

See also Expert settings.

## 12.1 Expert settings

Expert settings

Expert settings are for advanced users. Change them only at the direction of the technical support or developers.

Bluetooth scan time - the maximum time during which the application waits from the system for a response to a request to build a list of available Bluetooth devices. By default, it is 20 seconds. Under normal conditions, when the device is working properly, is near the phone and there is no interference, scanning for Bluetooth devices is much faster and there is no need to adjust the scan time.

Connection timeout: The time during which the application waits for a connection to the device. If the connection is unstable, you can try to increase this time.

Location request rate: The desired interval at which the application receives location information from the system. This time is an approximate one and the system can inform the application about the change in location either more often or less often than the specified interval. Increasing the interval saves battery life on your smartphone, decreasing the interval may make location determination more frequent (which can be important when traveling at high speeds), but it will drain the battery faster.

Use legacy Google Maps renderer: Google announced the availability of a new, improved map renderer. If you disable the "Use legacy Google Maps renderer" option, then  
the RadiaCode application requests the use of a new renderer. However, when using the new renderer, map rendering is often noticeably slower. The effect of changing the value of this option appears only after restarting the application.

“Debug” group settings are associated with debug information that is written to the application log file in diagnostic mode. The developers may ask you to enable this or that option in order to better understand the problem that has arisen. All of these options are disabled by default. enabling them significantly increases the size of the log file and can affect application performance. After enabling debug options, you need to restart the application.