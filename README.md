No longer need to edit JS code.  Use case module to set/clear holidays that are derived from the JS code. 
The 3 modules, the case, set, and clear modules can be moved to parent IVRs for cases where varying 
BU’s have different holidays (i.e. integrators, etc).  Test Holiday is now fixed at 12/25/2022 so you only
need to set the testmode to 1 to test functionality. 
 
The observed value can now be set to 3 condistions. 
0 – Only actual holidays are set 
1 – Actual and observed holidays are set (Friday prior to Saturday and Monday following Sunday). 
2 – only Monday following Sunday is set to accommodate customer that are open on Saturdays and 
	and don’t observe on Fridays. 
	
Holidays Supported:
o	New Years Day
o	Martin Luther King Day
o	Valentines Day
o	Presidents Day
o	Good Friday
o	Tax Day
o	Easter Sunday
o	Mothers Day
o	Memorial Day
o	Fathers Day
o	Juneteenth
o	Independence Day
o	Parents Day
o	Labor Day
o	Grandparents Day
o	Columbus Day (Indigenous peoples day)
o	Veterans Day
o	Thanksgiving Eve
o	Thanksgiving Day
o	Black Friday
o	Christmas Eve
o	Christmas Day
o	New Years Eve
o	Any other day will see 'holiday' = 'No Holiday'

Variable 'isHoliday' will equal 'true' or 'false' depending on whether today's date matches one declared in the function.

## Version Changelog
* 1.0 Initial release
* 1.1 Modified line 55 to change the default test format from ("yyyy-mm-dd") to (yyyy,mm,dd) where mm starts at 0 for January, 11 for December. When using ("yyyy-mm-dd"), sometimes the function would apply a timezone offset which could change the date.
* 1.2 Current release: added Juneteenth (technically June 19) and Tax Day (typically April 15), with the additional handling of when these fall on a Saturday or Sunday, the observed date is adjusted from Saturday to the preceding Friday and Sunday to the following Monday.
