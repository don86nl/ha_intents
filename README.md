# Home Assistant Assist Timer Functionality.
This script adds timer functionality to Home Assistant's Assist.
For now, it adds the ability to start and stop timers and ask how much time is left on all or a specific timer.

# Usage
This script uses timers, input_booleans, a script and an automation.

#Installation
HELPERS
Create 3 timers; timer.timer1, timer.timer2, timer.timer3.
Create 3 input_booleans; input_boolean.timer1, input_boolean.timer2, input_boolean.timer3

FILES
Add the content of scripts.yaml to your own scripts.yaml.
Add the content of automations.yaml to your own automations.yaml file.
Add the folder 'custom_sentences' to your installation.
Add the file config_assist_intent_script.yaml to your installation or add the content of the file to yours if you already have such a file.

RESTART
Restart your Home Assistant instance.

# FAQ
# Why input_booleans?
Assist waits for the called service to complete before giving an answer. This means that when a timer has been stopped, Assist's answer will be given without that timer's status.
For example, we ask Assist to stop a timer. The service will stop the timer, then Assist will tell there are no timers active (instead of 'Okay, stopping the timer).
This will be resolved when timers get a response feature (like the conversation process has now).

# Why scripts?
If the intents uses the timer services, you cannot cancel the service if an error has been made. For example, if no timer has been specified, but multiple timers are active.
Using scripts, if this happens, the script stops. The Assist response will be that there are multiple timers active and the specific timer should be mentioned.
