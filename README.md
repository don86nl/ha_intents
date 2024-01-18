# Home Assistant Assist Extra Functionalities.

# 1\. Goodnight routine

This package adds a customizable routine to your Assist for when you go to bed!

## Usage

**Installation.**
*If this is your first package for Home Assistant, then add the following line to your configuration.yaml:*
`homeassistant:`
`  packages: !include_dir_named packages`

1.  Place the package folder (if you don't have one yet) in your Home Assistant /config folder.
2.  Place the language of your picking in your *config/custom_sentences* folder.
3.  Modify the package file to your preferences.
4.  Restart Home Assistant.

# 2\. Timers

This script adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start and stop timers and ask how much time is left on all or a specific timer.

# Usage

Installation

1.  TIMERS

- Create 3 timers; timer.timer1, timer.timer2, timer.timer3.

2.  FILES

- Add the folder 'custom_sentences' to your installation.
- Add the file config\_assist\_intent_script.yaml to your installation or add the content of the file to yours if you already have such a file.

3.  RESTART

- Restart your Home Assistant instance.

# FAQ

1.  Why delays?
    Sometimes Assist is slower in its answer than the service performing the action.
    For example, we ask Assist to stop a timer. The service will stop the timer, then Assist will tell there are no timers active (instead of 'Okay, stopping the timer).

# Known bugs

1.  When stopping a timer, Assist currently responds with 'that timer is not running'. The timer(s) is/are stopped nonetheless.
