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

**2\. Timers**
THIS SCRIPT WILL BE UPDATED TO BE USED WITH PACKAGES! DO NOT USE AT THIS MOMENT!

This script adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start and stop timers and ask how much time is left on all or a specific timer.

# FAQ

1.  Why delays?
    Sometimes Assist is slower in its answer than the service performing the action.
    For example, we ask Assist to stop a timer. The service will stop the timer, then Assist will tell there are no timers active (instead of 'Okay, stopping the timer).

# Known bugs

1.  When stopping a timer, Assist currently responds with 'that timer is not running'. The timer(s) is/are stopped nonetheless.
