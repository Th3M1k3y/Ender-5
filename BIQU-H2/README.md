## BI-QU H2 adapter without BL Touch

![Without BL Touch](https://raw.githubusercontent.com/Th3M1k3y/Ender-5/main/BIQU-H2/ender5_biku_h2.png)

## BI-QU H2 adapter with BL Touch

To define the probe position, on the BTT RRF board, you can use this. Increase the Z value for G31 to move the nozzle closer to the bed, or decrease it to move it further away.
```
M950 S0 C"servo0"                              ; create servo pin 0 for BLTouch
M558 P9 C"^probe" H5 F120 T6000                ; set Z probe type to bltouch and the dive height + speeds
G31 P500 X32 Y-1 Z1.77                         ; set Z probe trigger value, offset and trigger height
M557 X35:215 Y10:200 P9:9                      ; define mesh grid
```

[Buy me a coffee! ☕](https://www.buymeacoffee.com/mikeydk)
