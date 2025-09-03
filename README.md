Hi! 

This code originated from Amanda working with the HID study. The purpose was to simutaneously start multiple OBS recordings.

I have modified it greatly to account for the issues the MDL team is having. This includes (1) syncing the audio and visual recordings, and (2) adding event markers.

The audio is recorded via OBS so setting up this script alone should sync the audio by having the video and audio start at the same time.

* Does not send to OBS : Chapter Markers

* Pull timestamp from OBS
    * Solves UTC timezone

* JSON input markers - Amanda

* Ask for input name for the file for a function

* If one of the devices is already recording...
    * keeps looping
    * Printing an error that failed to start all
    * timeout error