# web-hns-locator
Multipoint triangulation app for rocketry events. The idea is to load the web app on a phone and use the sensor and geolocation API to plot lines from multiple locations to triangulate a point in the distance, say a rocket that landed within sight far away or in a corn field. Sight lines grouped by time and converging within a small area can then provide a point that can be loaded in maps to easily get to a location.

Initial features planned:
 - Use Geolocation and AbsoluteOrientation Sensor APIs for shooting an azimuth from a GPS locked location.
 - Azimuths get cached locally on local storage until network/internet access is available to transfer stored lines to the server.
 - Support base stations that can import azimuths from custom hardware / mesh networks.
 - Allow inputing locations for tracked targets
 - Viewing shows plotted lines overlayed over a satellite or topographical map.
 - Add ability to select a specific target (rocket name?) if known
 - Can select groups of lines by time window, manually, or for a known target to be used for a triangulation
 - Triangulation provides LatLon to be easily used with other systems or to load into something like google maps.
 - Google Maps navigation within the triangulation app?
 - To shoot an azimuth, press a button to start a 3 second countdown to give time to line up with the target.
 - 3D printed sights that can be clipped to phones for higher accuracy?
 - Ensure a server and app can be run locally on a network and not require full internet connection.