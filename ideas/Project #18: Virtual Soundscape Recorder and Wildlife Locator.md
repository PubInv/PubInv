# Purpose

The sounds of nature are fascinating, particularly the sounds of anmials. It would be delightful to be able to record
a space for a given amount of time and then recreate the soundscape.

Imagine recording a section of forest in the springtime (in the Northern Hemisphere) when the songbirds are singing.
Then one would want to be able to physically or virtually walk into the space and listen (up close) to what you would
have heard if you could have been in a particular location.  What if that bluebird had been on your shoulder?

Passive Acoustic Modelling (PAM) has also emerged as ann [ecosystem assessment tool](https://www.wildlabs.net/resources/case-studies/monitoring-ecosystems-through-sound-present-and-future-passive-acoustics) with significant potential to aid ecosystem service mapping, and baselining. Since each species in an ecosystem has co-evolved to fill a different part of the "symphony of sound", measurable and quantifiable as the frequency domain, recordings of the symphony of sound prior to human contact help provide a baseline which must then be met through wildlife rehabilitation projects by prospective developers.  

Prior art also exists in ecoacoustics from [Rainforest Connection](https://www.rfcx.org/), who combines the audio sensors and cellular networkinng of post-consumer (used) cellphones, with power generation from solar cells, to deploy monitoring networks of offgrid embedded systems that send deforestation and poaching alerts, in addition to cataloguing ecoacoustic data.  

# Techniques

I belibe this should be accomplishable with an array of microphones.  Seismologist do this kind of think all the time.
The basic idea is to use the microphones as a "phased array" to create a directional mic.
However, we would be recording ALL fo the soundscape.

The problem might then become one of generating models that match the recorded signals (seismologist do this too.)
This would allow us to convert a set of recordings into concept "A songbird sat at 8 feet height on that tree and sang
like this:..." instead of simple recordings.

# Uses

In addition to its beauty, this could be used to study cryptic animals.  For example, the North American tree frogs
are poorly studied compared to the poison-dart frogs of Central America.  You could use this system for finding them. 
Possibly there are animals which are suspected but have never been identified which coudld be physically located with
this technique (I imagine that many of them would be arthropods, of course.)

# Notes

I really think of this as a Raspberry PI type project, not an Arduino project.  Nonetheless, the Arduino DOES have an (FFT library)[http://wiki.openmusiclabs.com/wiki/ArduinoFFT]. This would make it possibly to at least test out some ideas with an Arduino.

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">PIFAH Project #18: Virtual Soundscape Recorder and Wildlife Locator</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/PIFAH/PIFAH" property="cc:attributionName" rel="cc:attributionURL">Robert L. Read</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.<br />Based on a work at <a xmlns:dct="http://purl.org/dc/terms/" href="https://github.com/PIFAH/PIFAH" rel="dct:source">https://github.com/PIFAH/PIFAH</a>.
