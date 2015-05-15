# How to Control a High-Power Ray Gun with an Arduino

1. Get a Ray Gun (RG).
2. Decide how to power the RG. Batteries are portable. Up to 30A and 60V can be powered with the Fairchild Semiconductor
FQP30N06L for $0.95, as explained in a bildr.org [tutorial](http://bildr.org/2012/03/rfp30n06le-arduino/).
3. Get an N4001 diode to use as a flyback diode, since yoru RG might produce a back voltage. (TBD: I need to check if this is really a well-rated diode for this circuit.)
4. Build the circuit:

Wear your safety goggles when cutting wire or soldering. Remember, use Red wires for power, Black for ground, and other colors for everything else. I like Green for important signal wires.

5. Test your ability to fire by applying 5V to the green wire.
6. Choose a sensor, such as a Hidden Hostile ExtraTerrestrial Probability Detector. If an HHETPD is hard to source,
consider starting with a switch, a pressure trigger, or a temperature sensor such as those provided by the Arduino
Experiment Kit (ARDX)[http://oomlout.com/a/products/ardx/].
7. Most sensors require 5V and GND provided by your Arduino, and produce a voltage. Wire your sensor to your Arduino,
using A0 for the input. It will probably look like this:

8. Wire your Arduino output pin 0 to the green wire of RG.
9. Run this simple sketch in your Arduino:

10. Test your poject in Debug Mode so you can see your sensor reading.

11. Package your project so it is waterproof, sturdy, and kid-safe. It might looks like this:

* Test your packaging for usability just as much as you tested your electronics.
* Use plug connectors if you want to reuse parts of your project.
* Use Stranded wire fore moving joints, but don't count only on solder connections to keep wires in place.
* Add indicator LEDs to your project in case so you can get some information when are connected to a computer.

12. Here are two examples Ray Gun controller repurposed:
* Infant warmer
* Anti-stink fan

## References

* "High-Power Control: Arduino + N-Channel MOSFET" http://bildr.org/2012/03/rfp30n06le-arduino
* Adafruit ARDX - v1.3 Experimentation Kit for Arduino (Uno R3) - v1.3 http://www.adafruit.com/products/170
* We are planning to produce the circuit above as a sharable PCB design. Look for it at the Engineers Without Borders GitHub 
[repository](https://github.com/PIFAH/EWB)
* http://www.instructables.com/id/Yet-Another-Arduino-110v-Power-Controller/
