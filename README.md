# IVR-USA-Holiday-Auto-Detect
This IVR supports automatic calculation of USA holidays.

Use case: import this IVR into Virtual Contact Center, call it from other parent IVRs, return to the calling IVR optionally two variables: 1) isHoliday and 2) holiday. The variables are then used in the parent IVR to support either generic or specific holiday functionality

Supported Holidays (exactly the value returned by variable 'holiday'):
* New Years Day
* MLK Day
* Presidents Day
* Valentines Day
* Easter (also Good Friday)
* Mothers Day
* Memorial Day
* Fathers Day
* Independence Day
* Labor Day
* Columbus Day
* Thanksgiving (also Black Friday)
* Christmas Eve
* Christmas Day
* New Years Eve
* Any other day will see 'holiday' = 'No Holiday'

More generically, variable 'isHoliday' will equal 'true' or 'false' depending on whether today's date matches one on the list.

[Watch the howto video](https://fivn-my.sharepoint.com/:v:/g/personal/jsosebee_five9_com/EVVSIL-g35JKlP1k89gBB7sBjvWTPOaMVcNdPjY0DUU47g)
