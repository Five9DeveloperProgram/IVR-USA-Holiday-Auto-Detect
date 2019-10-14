# IVR-USA-Holiday-Auto-Detect
This IVR supports automatic calculation of USA holidays.

**Use case**: import this IVR into Virtual Contact Center, call it from other parent IVRs, return to the calling IVR optionally two variables: 1) isHoliday and 2) holiday. The variables are then used in the parent IVR to support either generic or specific holiday functionality.

Supported Holidays (exactly the value returned by variable 'holiday'):
* New Years Day
* MLK Day
* Presidents Day
* Valentines Day
* Good Friday
* Easter
* Mothers Day
* Memorial Day
* Fathers Day
* Independence Day
* Labor Day
* Columbus Day
* Thanksgiving
* Black Friday
* Christmas Eve
* Christmas Day
* New Years Eve
* Any other day will see 'holiday' = 'No Holiday'

Variable 'isHoliday' will equal 'true' or 'false' depending on whether today's date matches one declared in the function.

## Recorded Instructions
[Watch the howto video](https://fivn-my.sharepoint.com/:v:/g/personal/jsosebee_five9_com/EVVSIL-g35JKlP1k89gBB7sBjvWTPOaMVcNdPjY0DUU47g)

## Download
1. [Click here to download the ZIP archive](https://github.com/Five9DeveloperProgram/IVR-USA-Holiday-Auto-Detect/blob/master/checkHoliday.zip?raw=true)
1. Secondly, open a new IVR in the editor > Actions > Restore > choose the checkHoliday.zip file from step one > Restore
1. Enjoy USA auto-detected holidays!

## Warning!
**Do not** forget to re-comment out line 55 of the function once testing is complete.
