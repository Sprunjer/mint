# mint
Private hub for direct content handling.

Section "Monitor"
    Identifier             "Monitor0"
EndSection

Section "Device"
    Identifier             "Device0"
    Driver                 "vesa" #Choose the driver used for this monitor
EndSection

Section "Screen"
    Identifier             "Screen0"  #Collapse Monitor and Device section to Screen section
    Device                 "Device0"
    Monitor                "Monitor0"
    DefaultDepth           16 #Choose the depth (16||24)
    SubSection             "Display"
        Depth              16
        Modes              "1024x768_75.00" #Choose the resolution
    EndSubSection
EndSection
