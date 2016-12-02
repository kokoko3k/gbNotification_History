gbNotification_History
======
Monitor dbus notifications and stores them forever

Plasma 5 does not keep unread notifications forever anymore.
If you miss that, read on.

This tool sits in the system tray and uses dbus-monitor 
to intercept and store notifications internally, forever.
They are not blocked, just "copied".

When you click on the tray icon, it will just send the stored
notificationw to the system notification daemon again, but it will
change the duration so that tey will be persistent.


Mandatory requirements:
======
  * dbus-monitor
  * system tray 
  * Qt5 (it is possible to use Qt4 with little effort)
  * Gambas 3 (usually the very latest version)


Compiling it:
======
```
After you installed gambas 3, just checkout and compile xt7 that way:

# git clone https://github.com/kokoko3k/gbNotification_History
# cd gbNotification_History/
# /path/to/gambas/binaries/gbc3 -e -a -g -t -p -m
# /path/to/gambas/binaries/gba3
# ./*.gambas
```

