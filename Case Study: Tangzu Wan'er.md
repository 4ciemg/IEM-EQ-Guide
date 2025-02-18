---
order: 97
icon: sliders
---
# Case study: Tangzu Wan'er

Now that EQ and other forms of DSP have been covered, it is time to apply what was learned; in this guide, the Tangzu Wan'er will be the IEM of choice due to its popularity. Note that the following steps will only use a few of the sections, mainly the ones that have time-efficient steps (ie not ones that require a lot of time). Those included should be relatively easy, accessible, and effective enough for most people. 

!!!info Personal preference and perception
- Bass has to be present in ample quantity. Sub bass is important, but not as much as mid bass presence and "punch"
- Mids have to sound natural. Maximum of the ear gain has to be between 2.5 and 3 kHz. The fine details depend on the rest of the FR. Some coloration is acceptable in the lower mids to accentuate the rest of the mids
- Treble has to be present and will, in most cases, be slightly higher in amplitude compared to targets like JM-1 
- Imaging and soundstage is mostly the same across IEMs 
- Listening volume around 60-70 dB in very quiet environments (<40 dB)
!!!

***
## Data 
The following FR graph shows the insertion depth profile for the Wan'er in order to reveal treble level as well as other possible unwanted resonances. Note that different sizes of the same tip (silicone, medium size bore) were used to achieve these measurements. As insertion depth gets deeper, pushing the coupler's resonance peak higher in frequency, it becomes clear that the treble on the Wan'er slopes down rather aggressively, which might not have been too obvious with an 8 kHz aligned resonance measurement. Furthermore, since 711 measurements are inaccurate in the treble region, the need for measurements of different ear tips isn't crucial; in my case, I found tips that were comfortable and used them when using EQ by ear (stock black bore tips). 

![Tangzu Wan'er insertion depth profile](https://i.postimg.cc/Hj17Dw0H/Waner-Insertion-Depth.jpg)

For the bass, everything looks fine, but remember that 711 measurements often overestimate this region, and are inaccurate when it comes to recreating proper sealing/leakage of IEMs with actual ear canals. While the graph might indicate a normal amount of bass, actual bass response in my ear might be (and actually is) different, and **much lesser than what was measured**. The distortion profile is also fine, measured at around 104 dB with most of the frequency range having less than 0.5% distortion limited to second harmonic distortion; as mentioned previously, distortion for IEMs is almost always negligible, even with very large EQ changes, and the same applies to the Wan'er.

!!!info Summary of Tangzu Wan'er impressions and EQ goals
- Bass is on the lacking side in terms of "punch" and overall "technicalities", but the overall balance is good
- Treble needs some more quantity, and there are a few peaks that should be addressed 
- Mid range is good, but there is a slight "closed in" presentation, and vocals are emphasized
- EQ will be used to improve bass quality, fix treble, and minimize the perceived "closed in" presentation
!!!

***
## EQ

For bass, as mentioned previously, a significant boost is needed; knowing my personal preferences, three filters will be used. The first one is a peak filter at 20 Hz with a Q of 0.5 for sub bass. The second is a low shelf filter at 100 Hz with a Q of 0.71 for more "impact" and presence in the track. Finally, a peak filter at 200 Hz (or any region depending on preference) with a Q of 1 is used to prevent any possible excess lower mids and mid bass bleed while accentuating the bass quantity/quality as well as the rest of the FR. For the gain values, it depends on what the goal is. In my case, small gain values were enough to improve bass qualities instead of shifting the overall tonal balance; for the first two filters, 2 dB was enough, and for the last, -2 dB.

For my own preference, treble will need to be slightly boosted; in this case, with a high shelf filter starting at 6 kHz with a Q of 0.71. The gain can be changed at any time, and is not a big concern for now. The second step will be to check if there are big resonances for my individual perception. With a tone generator, I located two very significant resonances; one at 7.1 kHz, another at 10.3 kHz, and a last one at around 14 kHz, all of which were audible with music and were cut down with peak filters with a Q of 4. Now that they've been identified, **pink noise and music** was used to determine the gain. With only the tone generator and aiming for relative/roughly equal loudness, both needed -8 dB, which resulted in music sounding muted. With music and pink noise, the first peak could be decreased by -4 dB, leaving a bit of extra "sparkle" without sounding harsh. The second peak could be set at -6 dB, while the third one wasn't audible on most tracks, but a -2 dB cut can be used to be on the safe side.

Finally, for the mid range, most of it sounds good. Since the ear gain is mostly positioned correctly (would have preferred for it to be closer to 3 kHz) and the rest of the mid range from 300 Hz to 1 kHz sounds fine, there is little to modify, especially when considering that most of the previous changes address the transition ranges. A potential issue is the lack of separation and "closed in" feeling, which is most likely due to excess energy from 1-2 kHz caused by an early ear gain. Using a 1.5 kHz filter with a Q of 1 can be useful, and a gain of -2.5 dB seems to help effectively with separation and pushing vocals back in the mix, although personally the trade-off of having more vocal presence is fine for me as well.

Now that most "issues" in the treble and mid range have been addressed, the high shelf filter at 6 kHz seems to work best at around 2 dB. With the main changes set in place, small changes can be implemented for improving the intangibles. In this case, a small boost (1.5 dB with a Q of 1.5) at 9.4 kHz seems to accentuate perceived "resolution" while not altering overall tonality too much, and a small narrow boost around 2.7-3 kHz seems to increase perceived vocal details (too track dependent for so this will be ignored).

Below is the final FR of the Wan'er (measured with an 8 kHz coupler resonance) with the EQ filters. **Bold** filters are highly individual (ie only for me), and are excluded from the final FR; **every filter parameter should be modified to your preferences**. Preamp should be set to -4 dB.

![Tangzu Wan'er Final FR post-EQ](https://i.postimg.cc/TP5Gb4mN/Waner-Study-Case.png)

Filter type | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|
PK | 20 | 2 | 0.5 | 
LSF | 100 | 2 | 0.71 | 
PK | 200 | -2 | 1 |
PK | 1500 | -2.5 | 1 |
**HSF** | 6000 | 2 | 0.71 |
**PK** | 7100 | -4 | 4 |
**PK** | 9400 | 1.5 | 1.5 |
**PK** | 10300 | -6 | 4 |
**PK** | 14200 | -2 | 4 |

!!!note
**Of course, this is just a small example and doesn't include a lot of what was discussed throughout the guide. From just these small judgments and steps, the sound has been improved considerably without having needed to spend more than an hour to come up with this preset. Further improvements can be had in terms of bass quality and treble refinement, but stopping here would be perfectly fine as well.**
!!!
