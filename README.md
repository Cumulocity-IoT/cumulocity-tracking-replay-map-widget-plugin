# Cumulocity Tracking Replay Map Widget Plugin [<img width="35" src="https://user-images.githubusercontent.com/67993842/97668428-f360cc80-1aa7-11eb-8801-da578bda4334.png"/>](https://github.com/SoftwareAG/cumulocity-tracking-replay-map-widget-plugin/releases/download/1.0.0-beta/tracking-replay-runtime-widget-1.0.0-beta.zip)

The Cumulocity Tracking Replay widget is the Cumulocity module federation plugin created using c8ycli. This plugin can be used in Application Builder or Cockpit. The Cumulocity Tracking Replay widget help you to displays track lines of the tracking device with replay feature on map.


![tracking replay image](https://user-images.githubusercontent.com/83225057/120200287-ccd36180-c241-11eb-81b2-302d8ef993aa.png)

### Please note that this plugin is in currently under BETA mode.

### Please choose Tracking Replay Map Widget release based on Cumulocity/Application builder version:

|APPLICATION BUILDER | CUMULOCITY | TRACKING REPLAY MAP WIDGET PLUGIN  |
|--------------------|------------|------------------------------------|
| 2.x.x(coming soon) | >= 1016.x.x| 1.x.x                              |

## Features
*  **Tracking Events:** Displays the position in map at a particular time.

*  **Faster/ Slower:** Configurable speed for tracing the path movement.

*  **Date/Time Filter:** Filters tracking events based on the date/time selected.

*  **Marker Click:** Shows the longitude and latitude of the marker.

*  **Configurable Zoom:**  Select and configurable zoom which is best fit for your map.  

*  **Configurable Device:** Based on configuration during widget configuration a device can be selected. 

*  **Configurable Event And Fragment Type:** Based on configuration during widget configuration, events can be filtered to get only the desired type of event.

## Prerequisite
   Cumulocity c8ycli >=1016.x.x
   
## Installation

### Runtime Deployment?

* This widget support runtime deployment. Download [Runtime Binary](https://github.com/SoftwareAG/cumulocity-tracking-replay-map-widget-plugin/releases/download/1.0.0-beta/tracking-replay-runtime-widget-1.0.0-beta.zip) and install via Administrations(Beta mode) --> Ecosystems --> Applications --> Packages 

### Local Development?

**Requirements:**

* Git
* NodeJS (release builds are currently built with `v14.18.0`)
* NPM (Included with NodeJS)

**External dependencies:**

```

"angular-resize-event": "^1.1.1"

"leaflet2": "npm:leaflet@1.7.1"

```

**Instructions**
1. Clone the repository: 
```
git clone https://github.com/SoftwareAG/cumulocity-tracking-replay-map-widget-plugin.git
```
2. Change directory: 
```
cd cumulocity-tracking-replay-map-widget-plugin
```
3. Install the dependencies: 
```
npm install
```
4. (Optional) Local development server: 
```
npm start -- --shell cockpit
```
5. Build the app: 
```
npm run build
```
6. Deploy the app: 
```
npm run deploy
```

## User Guide

*  **Target assets or devices:** User can select a device. Based on device, list of devices will be display on Map. Only those devices are visible on map where position attributes are configured. 

**Tracking Replay Map On Screen Options:**
 
* **Filters**:  The following filters can be used to filter/get data for the specified time period:
	*  **Start Date/Time**
	*  **End Date/Time**
	*  **Last minute**
	*  **Last hour**
	*  **Last day**
	*  **Last week**
	*  **Last month**

  *  **Slower**: Reduces the marker speed to half.
  *  **Play/ Pause**: Marker traces the path when played and can be paused at any instance.
  *  **Faster**: Increase the marker speed to double.
  *  **Reload**: Useful for force reload/refresh map.
  *  **Zoom in/ out** : Zooms in/out of the map.

------------------------------

These tools are provided as-is and without warranty or support. They do not constitute part of the Software AG product suite. Users are free to use, fork and modify them, subject to the license agreement. While Software AG welcomes contributions, we cannot guarantee to include every contribution in the master project.
_____________________
For more information you can Ask a Question in the [TECH Community Forums](https://tech.forums.softwareag.com/tag/Cumulocity-IoT).
