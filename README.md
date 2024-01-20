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
[![Watch the video](https://img.youtube.com/vi/ebFY_aTDBQI/hqdefault.jpg)](https://www.youtube.com/embed/ebFY_aTDBQI)

**1\. Good night routine**
This package adds a (customizable) good night routine to your Assist functions.
When you say 'good night', assist will trigger several (chosen) actions, like turning off lights and telling open doors and/or windows.
*Disclaimer: The Google TV in the video was shutdown using the Google Assistant SDK, not the media_player.turn_off service call, which unfortunately doesn't work for this type of device.*

*You like the routine? Please consider voting for me in the Voice Assistant contest :) 
https://community.home-assistant.io/t/voice-assistent-contest-assist-goodnight-routine-for-everyone*

**2\. Set (bedside) alarm**
This package adds a (customizable) bedside alarm to your Assist functions.
You can ask it to set an alarm for a specific time. An automation is included which either plays a tts or media file on a chosen media_player when the spoken time is reached.
*Be sure to set the variables. You must specify a media_player or the routine won't work.*

**3\. Timers**
THIS SCRIPT WILL BE UPDATED TO BE USED WITH PACKAGES! DO NOT USE AT THIS MOMENT!

This script adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start and stop timers and ask how much time is left on all or a specific timer.

# FAQ

1.  Why delays?
    Sometimes Assist is slower in its answer than the service performing the action.
    For example, we ask Assist to stop a timer. The service will stop the timer, then Assist will tell there are no timers active (instead of 'Okay, stopping the timer).

# Known bugs

1.  When stopping a timer, Assist currently responds with 'that timer is not running'. The timer(s) is/are stopped nonetheless.
