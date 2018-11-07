# Home Assitant Configuration

Welcome to my Home Assistant Configuration.   If you haven't come across Home Assistant before, you really should check it out first. You can find it at https://www.home-assistant.io/.

My Home Assistant Configuration is a work in progress and is subject to change on a whim.  It's here for your inspiration or for use as an example. 

## Software Ecosystem

* HomeAssistant running on a Raspberry PI 3 using ArchLinux
* Various docker images running on a "server"
  * MariaDB (mysql) Database
  * MotionEye (cameras)
  * Facebox (Face detection)
  * Mosquitto MQTT broker
  * AppDaemon
  * Tasmoadmin
  * Node-Red
  * Plex
  * Sonarr
  * Radarr
  * NZBGet
  * Transmission
  * GitLab

## Smart Home Devices

* Google Home
* Sonoff Basic

## TTS and Extras

* Google TTS

## Device Tracking

* Network Ping
* GPSLogger

## Weather

* Darksky
* Sun/Moon

## Additional Features

* Floorplan

# FLOOR PLAN

pkozul's ha-floorplan is configured, as per his instructions at https://github.com/pkozul/ha-floorplan.

I generated my floorplan.svg using InkScape on Linux.

* Trace the basic wall layout of the house from an existing format.
* Paste SVG objects from other floorplans, such as couches
* Find relevant icons on Material Design Icons
* Assign HA IDs to the relevant SVG Objects

# SECRETS

The secrets.yaml.dist file is generated on updates of my secrets file and does
not contain any values, only the keys.  This can be used as a starting point
for using HA Secrets.

Additionally some files are included from a 'secret' directory; these will
ultimately be migrated to the secrets.yaml file.

# ZONES

Configuration includes some sample zones for nearby places that are frequented,
if you wish to override your 'home' and 'work' zones, create files in the 
'zones' directory.

Additional "secret" zones are not included in this repository and are prefixed
as secret_* in the filename.
