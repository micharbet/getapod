GETAPOD
=======

The script that downloads Astronomy Picture Of the Day
------------------------------------------------------

**What it does**

- creates $HOME/apod folder on first run
- Downloads html page, then extracts image from the link
- keeps an history of last 14 days
- current image is linked like $HOME/apod/today.jpg

*best to be run from crontab:*
0 8,10,15 * * * /home/mich/bin/getapod >/home/mich/apod/getapod.out 2>&1
Then point your desktop background to the downloaded image (today.jpg) or you can setup slideshow from the whole directory

**What it doesn't**
- Images only, not another content like videos, flash, etc. supported
