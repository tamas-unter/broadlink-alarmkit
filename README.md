# broadlink_alarmkit
A fork from @nick2525's broadlink_s1c_s2c that has been fixed to work with Home Assistant 2026.9.4 - the new python library.

Here are the basic changes I made to avoid loading errors:

* imported async
* replaced the async decorator 2 locations and "yield from" to "await" 1 location
* edited the ha ALARM-related constants to match the updated SERVICE_ALARM syntax
* removed value 0 from the SOS state as key fob kept returning to SOS

original code: https://github.com/nick2525/broadlink_s1c_s2c
