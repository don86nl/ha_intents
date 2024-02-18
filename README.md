# Home Assistant Assist Extra Functionalities.

## Installation

If this is your first package for Home Assistant, then add the following line to your configuration.yaml:

`homeassistant:`

`  packages: !include_dir_named packages`

1.  Create a package folder (if you don't have one yet) in your Home Assistant /config folder.
2.  Place the package you wish to use *(for example 'packages/assist_goodnight.yaml' in this folder)*.
3.  Place the corresponding language of your picking in your *config/custom_sentences* folder.
4.  Optional: Modify the package file to your preferences.
5.  Restart Home Assistant.

## Available packages
[![Watch the video](https://img.youtube.com/vi/vAai49WE460/hqdefault.jpg)](https://www.youtube.com/embed/vAai49WE460)

**1\. Good night routine**
This package adds a (customizable) good night routine to your Assist functions.
When you say 'good night', assist will trigger several (chosen) actions, like turning off lights and telling open doors and/or windows.

*Available in Dutch, English, German and French language.*

*Disclaimer: The Google TV in the video was shutdown using the Google Assistant SDK, not the media_player.turn_off service call, which unfortunately doesn't work for this type of device.*

*You like the routine? Please consider voting for me in the Voice Assistant contest :) 
https://community.home-assistant.io/t/voice-assistent-contest-assist-goodnight-routine-for-everyone*

**2\. Set (bedside) alarm**
This package adds a (customizable) bedside alarm to your Assist functions.
You can ask it to set an alarm for a specific time. An automation is included which either plays a tts or media file on a chosen media_player when the spoken time is reached.

*Be sure to set the variables. You must specify a media_player or the routine won't work.*

*Available in Dutch and English.*


**3\. Timers**
This package adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start, pause, resume and stop timers. You can also ask Assist how much time is left on all or a specific timer.

*Be sure to set the variables in the package file. You must specify a location and default media_player in the first two lines.*

# Known bugs

1.
  You can ask assist to stop a timer which isn't running. It will always answer like it is stopping it. Unsure why this is happening...
