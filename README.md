# aduro
Control system for flame effects or other systems controlling 120v circuits.

Aduro provides the ability to switch a series of 120 volt sockets on and off remotely. Timing is rather important as is reliability, having a flame effect trigger at an inappropriate time can have rather dire consequences. 

General features of the system:

  - master control panel
    - simple interface
      - series of on / off switches, slider potentiometers and rotary potentiometers
      - or a touch screen?
    - programmable sequences
    - wireless communication with control packs
    - secure communications
    - control packs are registered with the control panel
      - there's a unique id for each control pack (uuid? mac address? other hardware serial number?)
      - capabilities included with registeration
  - secondary control interface
    - controllable via iphone / ipad / android tablet
  - control packs
    - quad 120v circuits pack controlled through relays
    - quad relay pack with exposed connectors
    - control packs return to a known state when communication with the maser controller is lost
  - other thoughts
    - logging of all commands


Possible hardware platforms:

  - master control panel
    - raspbetty pi 2
    - touch screen
  - control pack
    - relay board (http://www.ebay.com/sch/i.html?_from=R40&_trksid=p2050601.m570.l1313.TR0.TRC0.A0.H0.Xrelay+board.TRS4&_nkw=relay+board&_sacat=0)
  - wireless communications
    - xbee / zigbee (https://www.sparkfun.com/products/10421)
    - 802.11x wifi
    - pinoccio arduino (https://docs.pinocc.io/)
    - particle photon (https://www.sparkfun.com/products/13774)
