# einkhole

This is a quickly hacked-together Python script for displaying pihole statistics on a Waveshare 2.13 inch e-ink display plugged in as a hat on my Raspberry Pi Zero 2 W. 

I've forked and modified some aspects of this repo/script from dozer55. So all credit for the original implentation goes to him. 


1. Set up the display as described in the Waveshare resources and use the test examples before installing my script (resource link below)
2. (optional if not using step 1) Use install_libs.sh to install all required libraries for the waveshare display
3. Be sure to install all Python packages needed for the script to run
4. Customize to your heart's content!

To get this to refresh, I set it up with a cronjob to run every 30 minutes, which looks like: */30 * * * *

# Edit crontab

crontab -e

*/30 * * * * python /home/pi/einkhole/einkhole.py


Need help with cronjobs? Check out https://crontab.guru

# Waveshare Resources
There are fantastic resources for this display here:

https://www.waveshare.com/wiki/2.13inch_e-Paper_HAT


