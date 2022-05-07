+++
title = "socketMusic: airports"
date = 2019-07-05
description = "WebSockets installation version of airportmusic"

[extra]
author = "Derek Kwan"
thumbnail = "/thumbs/other/install/smasquare.jpg"
keywords = "socketMusic, airportmusic, airports, music of airports, ambient, Raspberry Pi, WebSockets, Tone.js, Node.js"
+++
_socketMusic: airports_ is an installation version of airportmusic that mashes the original fixed-media piece up with the ideas of socketMusic: wireless. In my concept of socketMusic, I have audience members connect to a router hooked up to a Raspberry Pi in this case and load a webpage hosted with Node.js. Through the magic of WebSockets (socket.io in the case of Node.js), I am able to target individual clients and trigger events on the devicse. This version takes the original mappings of Hong Kong International Airport departures and arrivals to synthesizer notes and airport and airplane samples respectively and distributes them to connected clients randomly. As this is meant as an installation, the day loops back to 0:00 when the end is reached. 

![sma-install-sm](/images/other/install/sma-install-sm.jpg) \

<iframe width="560" height="315" src="https://www.youtube.com/embed/3kf1Z3L-i48" class="embedplay" frameborder="0" allowfullscreen></iframe><br>
