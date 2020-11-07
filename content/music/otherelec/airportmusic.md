+++
title = "airportmusic"
date = 2016-01-01
description = "fixed-media sonification of Hong Kong airport arrivals and departures"

[extra]
author = "Derek Kwan"
keywords = "sonification, fixed, pure data, audacity, airport, eno"
+++
_airportmusic_ (2016) stems from my long-standing fascination with networks of transportation and is the expansion of the ideas behind Brian Eno's Music for Airports. With airportmusic, I wanted to create music not just for airports, but by and of airports. The piece is a sonification of the arrivals and departures of planes at Hong Kong International Airport on Decemeber 4, 2015 beginning at midnight with the duration of a 12/4/2015 hour mapping to thirty seconds in airportmusic. The departures are sonified by FM-synthesis instruments where the gate numbers correspond to pitch and are mapped diatonically to a major scale while the flight numbers correspond to the lengths of recirculating delay lines the notes are fed into. The duration of each note is fixed. The arrivals are sonified by Creative Commons-0 samples of airports and airplanes captured by Freesound.org users. Since the gate information was unavailable, the particular sample representing each arrival is chosen at random while the flight numbers this time correspond to the durations of notes. The speed and pitch at which each sample is played back are determined randomly and independently. All other aspects of the sounds such as the delay line lengths of the arrivals and the panning of both arrivals and departures are determined randomly. Furthermore, a CC-0 Freesound sample consisting of ambient airport noise that is stretched granularly throughout the piece up to ten times its original length provides a sonic backdrop. The left and right channels are often in sync with each other, but are also at times played back at separate rates. My sonification for airportmusic was realized through Pure Data. I retrieved the flight data from the HK Int'l Airport website and parsed the data using custom Python scripts. Although my musical choices are not the best for perceiving the data, they result in a more listenable musical experience and the density of arrival and departures can still be sensed.

I later adapted the piece as an installation hosted on mobile devices called [socketMusic: airports](/project/install/smairports.html).

<iframe style="border: 0; width: 100%; height: 120px;" src="https://bandcamp.com/EmbeddedPlayer/track=3688676307/size=large/bgcol=ffffff/linkcol=0687f5/tracklist=false/artwork=small/transparent=true/" seamless><a href="http://derekxkwan.bandcamp.com/track/airportmusic">airportmusic by Derek Kwan</a></iframe>
	
![airportmusic-pd](/music/images/airportmusicdep-pd.png) \
