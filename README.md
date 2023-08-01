# Home Assistant Assist Timer Functionality.
This script adds timer functionality to Home Assistant's Assist.

# Why scripts?
If the intents uses the timer services, you cannot cancel the service if an error has been made. For example, if no timer has been specified, but multiple timers are active.
Using scripts, if this happens, the script stops. The Assist response will be that there are multiple timers active and the specific timer should be mentioned.
