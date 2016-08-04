Battery Keeping
------------
Usually laptop batteries' life is measured in terms of number of charge/discharge cycles. In other words, after certain number of charge/discharge
cycles, batteries lose their charge holding capability and tends to charge quickly and drains super-quickly. One complete charge is called charge cycle and vice versa.


Problem statement
----------------
Batery life should be increased. The number of cycles should not be used up in no time.

Approach
-----------
Although I can't change the number of cycles of a battery,I can increase the period of each cycle. Plugging in & out the power chord before the battery falling below 30% and exceeding above 90% respectively can stop counting the charge/discharge as one complete cylce. BatteryKeeping application is based on this idea. Its monitors the battery level and the frequency of charge checking is managed by an algorithm based on the charge/discharge state, available charge, etc. 

It primarily uses batch files to communicate with wmic module to check the battery status. It has inherent capability to detect power chord/battery plugged/un-plugged status and starts/stops monitoring based on the detected status.
