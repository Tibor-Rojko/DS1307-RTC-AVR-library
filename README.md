# DS1307-RTC-AVR-library
Require once:

    rtc_Init();                 //Initialize the ds1307 module

    rtc_t rtc;                  //declare struct

    //Use your values
    rtc.hour = 15;              //Hour = 15
    rtc.min =  49;              //Minute = 49
    rtc.sec =  0;               //Second = 0
    rtc.date = 17;              //17th
    rtc.month = 1;              //Jan
    rtc.year = 19;              //2019
    rtc.weekDay = 7;            //Saturday: 7th day of week considering Sunday as first day.

    rtc_SetDateTime(rtc);	    //Setting the date and time of RTC module

Place it to the infinite loop:

    rtc_DateTime(rtc);		    //Reading date & time
