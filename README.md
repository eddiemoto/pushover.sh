pushover.sh
===========

Shell-script wrapper around curl for sending messages through PushOver

Usage
=====

    pushover.sh [-t <title>] [-d <device>] [-p <priority>] [-r <retry>] [-e <expire>] [-s <sound>] <message>
    
If you are using a priority of 2, the script will default with a retry value of 60 seconds and an expiration of 1 hour.  (-r "60" -e"3600")

Before you can actually use this script, you must create `${HOME}/.config/pushover.conf` with the following contents:

    TOKEN="your application's token here"
    USER="your user key here"


Shell compatibility
===================

A word of warning: The original author knows what he is doing... I do not.  First bash script I've really ever had to change.

