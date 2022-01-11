# TA-check-logFORj
Simple Splunk TA wrapper for https://github.com/stressboi/check-log4j which is forked from original Yahoo authors here: https://github.com/yahoo/check-log4j

This takes the script from the repo linked above and converts it into a scripted input for any Splunk Universal Forwarder running on a Linux server or endpoint. 

Simply drop it into the /etc/apps directory on a Universal Forwarder (or use deployment server or your favorite distribution method to get it there). By default it runs once an hour and sends the output with pre-pended timetamp into Splunk. It runs the main check script with no options which means it's scanning from the root of the filesystem - make sure this is what you want and if you don't want that, edit the inputs.conf file to change how it runs. Make sure the check-log4j.sh script is executable!

16DEC2021

brodsky@splunk.com
james.brodsky@gmail.com
