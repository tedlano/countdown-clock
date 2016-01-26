## Summary

A countdown clock written in HTML, CSS, JavaScript, and jQuery.  To change the countdown end time, open up countdown.js and edit the datetime string on line 72.

**Notes:**
* Works for user's current timezone.  Code will have to be updated if we want to account for timezone differences.
* When countdown reaches 00:00:00:00, alert message "Happy New Year!" shows up
* Found background image for numbers at http://www.jqueryscript.net/demo/Beautiful-jQuery-Countdown-Timer-Plugin/, sliced it into 3 parts using GIMP 2.  My code is different than the code available on this site.

**Tricky Parts:**
* Dynamic width of background number displays:  Since days can be >2 characters long, had to figure out a way to make the background image width for the number diplays dynamic.  Sliced up background image into 3 parts: left, middle, and right; and repeated middle section as necessary.
* White strikethrough in middle of numbers also had to account for variable width.

**Testing:**
* 2016-01-26 09:40: Wasn't working in Firefox or IE; solution: change input date format on line 80 of countdown.js from "2016-12-31 23:59:59" to "2016/12/31 23:59:59"