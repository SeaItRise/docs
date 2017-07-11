
# Core Features

## Map Mode
### Mandatory 
 * Show Map of local area
 * show current location with "beacon"
### Nice to Have
 * toggle between map view and satellite
 * show lat/lon
 * allow for setting of "pin" to mark location
 * show nearby pics already taken
 * show overlay of RSL NOAA layer
 * zoomable
 * searchable by address
 * show parcel level data? (this likely will cost $$)

## Tide Chart and Weather Mode
### Mandatory
* show closest NOAA tide gauge data in table and/or graph form
### Nice to Have 
 * show available weather (?)
 * show predicted storm surge (or not) over next 24 hours, along with current tidal height
  <--- need more details filled in here --->
  
## Augmented Reality and Photo Mode
### Mandatory
 * basic camera/video functionality
 * phone location/orientation information saved into EXIF of image and/or video equiv
 * "AR" mode button/switch that turns on a layer of sea level, complete with slider to move it up/down
 * toggle to display tide height as overlay?
 * ability to toggle in to "photosphere" mode 
 
### Nice to Have
 * pokemon go style "am I underwater" game play (e.g. if you are, a virtual wave column appears, with different fish in it depending upon how underwater you are expected. Toggles for "storm surge cat 1, 2, 3 etc" as well
 * some indication in the view of where other pics were acquired
 <--- need more details filled in here --->

## Backend Database
 * photo objects
 * some method of spatial query
 * automatic (?) grouping of all photos w/in 100m? 200m?
 * photo metadata available via API
 * unique key for every photo

## Web App (frontend webpage, no app needed)
 <--- need more details filled in here --->
 
# Object/Entities and metadata for each
## User
 * Google/Facebook identity auth
 * user settings (height?)
 * number of images uploaded
 * Group (e.g. Seattle Aq Beach Naturalists, Surfrider, Windemere, etc)
## Image -- basic
### Mandatory
 * unique key
 * location (lat/lon)
 * time of picture (UTC)
 * camera EXIF data (handset details)
 * Sensor orientation
 * picture height above ground (user option? derive from camera/phone sensor, eg. ARKit?)
### Nice to have
  * user that took it
  * permissions user assigned
  * tag
  * tide height from nearest guage
  * weather from nearest guage/wx station
  * user entered note
## Image -- photosphere
 * inherits picture basic 
 * adds form of photosphere (handset? 360 camera?)
## Image -- Video
 * inherits picture basic
 * adds beginning/end transect for photogrammetry type acquisition?
