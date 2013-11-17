Arduino-temperature-monitor-receiver
====================================

Dual channel temperature monitor (receiver)
/* This sketch receives a packet of data from another Jeenode (Arduino clone)
 via a RFMB12 868MHz Transciever, the packet contains two temperature values and
 the Battery level for the transmitter (powered directly from 3.7V lithium not via
 the regulator), it also displays the recievers battery voltage.
 The sketch waits for a transmission and then sleeps for 53 seconds and wakes up 
 waiting for another transmission then sleeps again after reception.
 Based on this blog post
 http://gadjetsblog.blogspot.co.uk/2012/05/remote-temp-sensing-with-glcd-and.html
 The display used is a 128x64 pixel graphical LCD.
 Note, this sketch requires the GLCDlib library from JeeLabs
 https://github.com/jcw/glcdlib
 */
