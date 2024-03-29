# IVR-USA-Holiday-Auto-Detect
This IVR supports automatic calculation of USA holidays.

**Use case**: import this IVR into Virtual Contact Center, call it from other parent IVRs, return to the calling IVR optionally two variables: 1) isHoliday and 2) holiday. The variables are then used in the parent IVR to support either generic or specific holiday functionality.

Supported Holidays (exactly the value returned by variable 'holiday'):
* New Years Day
* MLK Day
* Presidents Day
* Valentines Day
* Good Friday
* Tax Day (observed)
* Easter
* Mothers Day
* Memorial Day
* Fathers Day
* Juneteenth (observed)
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
[Watch the howto video](https://github.com/Five9DeveloperProgram/IVR-USA-Holiday-Auto-Detect/blob/master/Walkthrough.mp4?raw=true)

## Download
1. [Click here to download the ZIP archive](https://github.com/Five9DeveloperProgram/IVR-USA-Holiday-Auto-Detect/blob/master/checkHoliday.zip?raw=true)
1. Secondly, open a new IVR in the editor > Actions > Restore > choose the checkHoliday.zip file from step one > Restore
1. Enjoy USA auto-detected holidays!

## Warning!
**Do not** forget to re-comment out line 55 of the function once testing is complete.

## Version Changelog
* 1.0 Initial release
* 1.1 Modified line 55 to change the default test format from ("yyyy-mm-dd") to (yyyy,mm,dd) where mm starts at 0 for January, 11 for December. When using ("yyyy-mm-dd"), sometimes the function would apply a timezone offset which could change the date.
* 1.2 Current release: added Juneteenth (technically June 19) and Tax Day (typically April 15), with the additional handling of when these fall on a Saturday or Sunday, the observed date is adjusted from Saturday to the preceding Friday and Sunday to the following Monday.
