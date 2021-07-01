# chkcrontab
After having banged my head against the wall several times (and damaging the wall in the process) because some cron jobs would not run,
I discovered that "0/15" in the first column does NOT tell cron to run a job every 15 minutes but "*/15" does.

In order to prevent this from happening to me again, I whipped up this small script to check the syntax of a crontab.

You can call it with the path name(s) of one (or more) crontab(s) (eg "/var/spool/cron/crontabs/pi").
If you leave out the file name, the script will run on the output of "crontab -l".

Have fun!
