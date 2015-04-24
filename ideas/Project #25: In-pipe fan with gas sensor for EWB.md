# With Engineers Without Borders: Sensor-controlled in-pipe Latrine Fan

Note: I don't really consider this an "invention", a term I reserve for something novel and unobvious. Rather this is
a simple engineering project.  However, it is being done in cooperation with the Great Austin Chapter of Engineers Without Borders,
who are attempting to build a composting toilet/outhouse got for a local farm cooperative. I'm making it a project because
I want to forge alliances, cooperation and sharing with such groups, and to be able to have a place to document the work.

## Idea: Ventilation fan based on Methane/Hydrogen Sulfide Sensors

The EWB group previously identified a desire to have a ventilation fan for their compost pits based on some experience
they had with a different toilet. I came to this project late, and am just following their approach. The whole EWB team
is perhaps 50 people split into several groups. The instrumentation team is in charge of the sensor/fan project.

## Status: Bread-boarded Arduino with Working Motor Control

Combining two little circuit design/sketches in the Arduino Experimenters Kit (ADX) from Adrafuit or Sparkfun, I bread-boarded
an Arduino and wrote a sketch that uses the pressure sensor to turn on a motor for 3 seconds.  I have a Methane sensor and
and H2S (Hydrogen Sulfide) sensor on-order.  The MQ4 methane sensor is not pacakged in a way that you can breadboard.
I've orderd a "breakout board" which should allow me to solder to it to test it.

I've been told we are going to exhibit something at the upcoming Mini-Maker Faire in Austin on May 16-17th, so I would
like to improve this project by that time.

## Stories

* Publish photos and sketch of current work
* Order a 12V fan that I can control with a relay or transistor (I have MOSFET transistors that can switch a lot of power.)
* Get a piece of PVC pipe into which we can mount the fan and potentially the sensor.
* Breadboard so that I can use 12V power instead of the 5V Arduino power for the fan.
* Try to mount the fan inside the PVC.
* Add a manual switch to the circuit.
* Add (simulated) gas-concentration readouts to the sketch.
* Get a smaller Arduino and a separate enclosure for actually mounting on the fan.
* Build a perfboard version (not a breadboard!) for demonstrations
* Publish schematics, maybe even EagleCAD up a PCB?
* Get the MQ4 sesnor working, burned in and tested.
* Get ready for Mini-Maker Faire!
* Test in a real barn/latrine!
* Test on my compost pile!

## References

* A YouTube video of something similar: https://www.youtube.com/watch?v=VhKLuDcLnKM
* A circuit diagram for something similar: http://www.seekic.com/circuit_diagram/index441.html
* A not-very-well-documented project: http://hackaday.com/2012/11/19/bathroom-fan-that-switches-itself-on-when-it-gets-steamy-or-smelly/
* This firm seems to just use caps rather than in-pip solutions: https://www.roofvents.com/aura-fan-kit-flat-roof-mounted-exhaust-fan-4800-cfm-kit-includes-24-diameter-aura-vent-6-collar
* There exist Duct Fans that are alread in-pipe, maybe I can find a 4" one: http://www.homedepot.com/p/Suncourt-Corded-4-in-In-Line-Duct-Fan-DB204-CRD/203227157?cm_mmc=Shopping%7CBase&gclid=CjwKEAjw0-epBRDOp7f7lOG0zl4SJABxJg9qP4Uio9FMdzkf_jG-On3bK42qXETH70YwsbNP0ENgphoCUl7w_wcB&gclsrc=aw.ds
* Here's a 4" inline 12 volt blower: http://www.amazon.com/Inline-Blower-235-CFM-Volt/dp/B001JHJ0WW



<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #24: Very simple heat engine with bistable magnetic device</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>. 
