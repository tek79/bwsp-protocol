# bwsp-protocol
basement watchdog special plus connect monitoring protocol

Basement Watchdog Special+ Connect

BWSP-A


Non-standard use of USB A for 5v TTL serial

Pinout:

Red: 5V (BWSP-A controller provides)

Green (D+): TX

White (D-): Unused

Black: GND


1200 8N1



System Status:

00= ok/normal

01= pump activated

08= battery

09= battery, pump activated

20= power fail - automatically resets back to 00 when ac restored

21= power fail, pump was activated - automatically resets back to 01 when ac restored

48= battery

49= battery, pump activated

58= no battery/disconnected

59= no battery/disconnected, pump activated



Charge Status:

6= charged

4= float

3= trickle

2= charge off/operating



Sample messages:

1420  4 00

1360  4 00

Battery Voltage, Charge Status, System Status
