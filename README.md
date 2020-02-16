# syncthing-tray

Manage syncthing from an appindicator tray widget/thing.

## Overview and Ramblings

I used the rather lovely Syncthing to sync various directories between my
phone, laptop, desktop and home server.  I use it in preference to Dropbox,
which whilst brilliant, also has no privacy and you have to pay them for lots
of data.  I have lots of data.  I like privacy.  Therefore, I use Syncthing.

On my desktop, I just leave it running in the backgroup all the time.  It's
started from the i3 start up file and it just runs.  If I want to see its state
then I have to run a browser and look at it.  Not ideal, but bearable.

However, on my laptop, I tend not to run it all the time.  I probably should,
but when I'm on battery it uses too much power, so I'd like it off.  Obviously,
I forget when it is switched off as I don't have the visual queue.  So my use
case is:

* Indicator as to whether it is running or not.
* Indicator as to whether there is a sync issue.
* Ability to ignore a sync issue.
* Ability to see the status of the individual syncs.
* Ability to open the website on the configured browser.

I won't bother with GUI for the configuration; I'll just use a configuration
file which it can read from an obvious place.  The other bits are just
accessing the API on the local machine and show the output.
