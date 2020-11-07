+++
title = "Art-a-Hack: Dancedemic - Hieroglyph"
description = "biometric-enhanced live-streamed dance performance"
date = 2020-08-21

[extra]
author = "Derek Kwan, Art-a-Hack Team Razvan"
thumbnail = "/other/collab/thumbs/hierosq.png"
keywords = "dance, biometric, emotibit, artahack, dancedemic, pure data, touch designer, ableton, poetry"
+++

In July-August 2020, I participated in the remote hackathon [Art-a-Hack](https://artahack.io/) involved fellows from all over the world collaborating with [Battery Dance](https://batterydance.org/) in New York, NY. In this particular edition of Art-a-Hack entitled Dancedemic, the fellows, meeting principally through Zoom meetings and remote logging into a machine at Battery Dance's studios, split off into two teams with each team working with either of two of the company's dancers, Razvan Stoian and Hussein Smko. Throughout the course of the hackathon, the teams worked on projects to enhance the audiovisual aspects of the dance routines using software running on the Battery Dance machine and utilizing data from biometric sensors called [EmotiBits](https://www.emotibit.com/) each dancer was wearing. The final performances were streamed on August 21, 2020 on a plaform provided by [elektron.live](https://elektron.live/).

I was a part of the team working with Razvan, a dancer from Romania, and our project "Hieroglyph" featured poetry by Nichita Stănescu and portrayed the linguistic difficulties of moving to a new city where you don't speak the language. Vinay Khare generated the visuals using Touch Designer and I collaborated with Yurii Tymoshenko in creating audio for the dance with Yurii working in Ableton and me working in Pure Data.

The poems we used for "Hieroglpyh" were "Hieroglyph, "Unwords", and “Jacob Battles the Angel: Or, On the Idea of "You". Kat Mustatea made recordings of her reciting these poems in English and Romanian and gave them to me to chop up into shorter fragments. 

For our tripartite structure, I processed Kat's voice in various ways. In the first part, my contributions were sparse and let Yurii's melodic contributions take center stage. I used short fragments of Kat's speech and pitch shifted them within an octave above and below their normal range as well as altered the speed (separately from the pitch) at which they placed back between 0.01 and 2 times their original rate. For this part, I only used Kat's voice in English. In the second section, I used these short fragments a constant rhythmic pulse while occasional long fragments of unprocessed speech came through. For this part, I only used Kat's voice in Romanian. In the third section, I used medium-sized fragments indirectly. I detected their frequency content through [sigmund~] and mapped these frequencies and their strengths to sawtooth oscillators so that it would sound like her voice is being fed through a vocoder. Furthermore, I rounded these frequencies to those of a lydian scale so the voice fragments would become melodic swells. For this part, I used a combination of samples from the previous two parts.

Throughout "Hieroglyph", I used two readings: PPG-IR and EDA. In Part 1, the PPG-IR reading was responsible for controlling the maximum duration of the fragments while the EDA reading was responsible for controlling the chance of the fragment being fed through a stuttering effect (for a glitchy aesthetic). In Part 2, the PPG-IR reading controlled the chance that a sample would be played in its full duration and it would be played unprocessed. In Part 3, the PPG-IR reading was responsible for controlling the cutoff frequency of a low-pass filter the oscillators were fed through. In Parts 2 and 3, the EDA reading was responsible for the chance of a sample being controlled multiple times (fitted to subdivisions of the pulse in part 2). 

In addition to the low-pass filter, I fed the sound through Freeverb and delay lines with feedback. I automated some of their parameters (and also parameters controlling trigger rate) to give each part a dramatic contour.

For the performance, the data from the biometric sensors was sent via OSC to Ableton which in turns sent the data to my patch and Touch Designer. Furthermore, I sent UDP data of which sample I was triggering to Touch Designer in Part 2 so that Vinay could use that information to trigger different visuals.

For this edition of Art-a-Hack, Ellen Pearlman served as our director while Katie Larson played a major part in organizing everything. Andy McWilliams setup and managed the computer technology and camera in the Battery Dance studio. My team members included: Aline Martinez, Manik Perera, Natasha Desai, Ni Ni Than, Nuntinee Tansrisakul ('Nun'), Sukanya Aneja, Vinay Khare, Yuguang Zhang, Yurii Tymoshenko, Kat Mustatea, and Razvan Stoian.

<iframe src="https://player.vimeo.com/video/468289209" width="640" height="360" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe>

![hiero-sshot](/other/collab/images/hiero-sshot.png) \

Screenshot from the live performance

![hiero-pdpatch](/other/collab/images/hiero-pdpatch.png) \

Performance patch for "Hieroglyph"

![hiero-sshot](/other/collab/images/hiero-sshot.png) \

Video/data player I made in Pure Data to replay video with biometric data (Can be found [here](https://github.com/derekxkwan/pd-dancedemic-playergithub.com/derekxkwan/pd-dancedemic-player)

	
