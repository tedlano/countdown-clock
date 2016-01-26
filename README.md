## Summary

A countdown clock written in HTML, CSS, JavaScript, and jQuery.  To change the countdown end time, open up countdown.js and edit the datetime string on line 72.

Notes:
* Works for user's timezone.  Code will have to be updated if we want to account for timezone differences.
* When countdown reaches 00:00:00:00, alert message "Happy New Year!" shows up


Testing:
* 2016-01-26 09:40: Wasn't working in Firefox or IE; solution: change input date format on line 80 of countdown.js from "2016-12-31 23:59:59" to "2016/12/31 23:59:59"