Schedule Class
The Schedule object is necessary in creating coupon schedules or call schedules. Schedule object constructors have the following signature:

## Here we have generated a Schedule object that will contain dates between effective_date

termination_date with the tenor specifying the Period to be Monthly. The calendar object is
used for determining holidays. Here we have chosen the convention to be the day following holidays.
That is why we see that holidays are excluded in the list of dates.
    
The Schedule class can handle generation of dates with irregularity in schedule. The two extra
parameters firstDate and nextToLastDate parameters along with a combination of forward or
backward date generation rule can be used to generate short or long stub payments at the front
or back end of the schedule. For example, the following combination of firstDate and backward
generation rule creates a short stub in the front on the January 15, 2015
