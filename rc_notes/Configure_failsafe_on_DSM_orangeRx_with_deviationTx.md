## RX side
- Connect orangeRx with binding connector on the binding port
- Power on the orangeRx
- Then remove binding connector

## TX side
- go to *Model menu* -> *Mixer* -> *1-THR* -> *Fail-safe*
- set to value -125
- then go to *Model setup* -> *DSMX*
- click bind
_ then the failsafe value with be set to the RX

## GSC side
- go to cleanflight configurator Failsafe tab, *Valid Pulse Range Settings -> Minimum* to be the value slightly higher than the value when you turn off the transmitor. The value can be seen from Receiver tab.

