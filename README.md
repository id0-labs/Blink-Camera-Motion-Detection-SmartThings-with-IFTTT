# Blink Camera Motion Detection SmartThings with IFTTT
SmartThings Blink Camera System integration to enable Motion Detection

**************************** DISCLAIMER ****************************

THIS DEVICE HANDLER CAN NOT GUARANTEE PERFORMANCE WITH THE BLINK

SENSOR.  NO GUARANTEE OF PERFORMANCE FOR ANY USAGE IS PROVIDED.

**************************** DISCLAIMER ****************************

This series of device handlers enable the Blink Camera motion detectors for use in SmartThings for alerts, etc.  It is intended as a stop-gap measure since the original integration was deleted.  

# Description:

There are two files included:

  a.  Blink System ST-IFTTT.groovy.  This file creates a Blink System device that will allow arming and disarming of the Blink system through IFTTT.
  
  b.  Blink Motion Detector ST-IFTTT.groovy.  This file creates a Blink Motion Sensor device that, when received from IFTTT, will flag that the blink camera or cameras have detected motion.

# Installation

Installation is a manual IDE installation.  If you are unfamiliar with this, see the SmartThings IDE instructions on installation.  It follows the following steps.

  1.  Install the two device hander packages into the IDE at the "My Device Handler" tab.
  
  2.  Create the System Device in "My Devices" using the "Blink System through IFTTT" custom device handler.
  
  3.  Create a Motion Detector device in "My Devices" using the "Blink Motion Detector through IFTTT".  You may create one, one for each camera, one for each area, etc.
  
  4.  Go to your IFTTT account and create the following applets.  You will have to first enable the SmartThings devices in IFTTT (through the IFTTT SmartThings "settings" tab).
  
    a.  SmartThings (System Device) to Blink.  If System Device is turned on, then arm the Blink System.
    
    b.  SmartThings (System Device) to Blink.  If System Device is turned off, then disarm the Blink System.
    
    c.  (for each camera) Blink to SmartThings (Motion Detector).  If motion is detected, then turn on the Motion Detector.
