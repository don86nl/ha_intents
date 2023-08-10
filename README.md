# Home Assistant Assist Timer Functionality.
This script adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start and stop timers and ask how much time is left on all or a specific timer.

# Usage
#Installation
TIMERS
Create 3 timers; timer.timer1, timer.timer2, timer.timer3.

FILES
Add the folder 'custom_sentences' to your installation.
Add the file config_assist_intent_script.yaml to your installation or add the content of the file to yours if you already have such a file.

RESTART
Restart your Home Assistant instance.

# FAQ
1. Why delays?
Sometimes Assist is slower in its answer than the service performing the action. 
For example, we ask Assist to stop a timer. The service will stop the timer, then Assist will tell there are no timers active (instead of 'Okay, stopping the timer).

# Known bugs
1. When stopping a timer, Assist currently responds with 'that timer is not running'. The timer(s) is/are stopped nonetheless.
