---
order: 99
---
# Tanchjim Bunny

Let's now take a look at a different IEM, the Tanchjim Bunny DSP. It comes with a 5-peak-filter PEQ stored in a USB-C cable, ideal for using it outside. The context is now different, and will therefore influence the EQ and its intended goals. This case study uses other sections; always use what is best for your needs.

!!!info Preference & Context
- FR has to account for high background noise from public transit
- Both bass and treble have to be relatively elevated
- Only 5 peak filters are available for the DSP cable
- Timbre not as important due to noise, not looking for the best 
- Listening volume around 75-85 dB when outside
!!!

***
## Data 
The following FR graph shows the insertion depth profile for the Bunny (with no DSP). Assume for this case that the Bunny will be used with the deepest insertion, resulting in a slight tilt in the FR. **It is important to note that these measurements were taken by someone else**; for outdoor use, noise will be high and audible, which removes the need for very precise EQ. Using other measurements is fine if the conditions and goals don't necessitate personal measurements.

![Tanchjim Bunny insertion depth profile](https://i.postimg.cc/NF7krd20/Tanchjim-Bunny-Tangzu-Sancai-Regular-Narrow-Bore-Tips-Measurements-2.gif)

The bass is dominated by mid bass. When used outside, it is enough to be heard even with high noise, but there is a lack of sub bass resulting in underwhelming bass response that is too bloated. For now, keep in mind that lifting the sub bass might fix this issue.

The treble also needs work, as deep insertion creates a warm tilt by lifting low frequencies a bit, and reducing high frequencies significantly. More precisely, the region from 3 to 8 kHz feels recessed, resulting in a dark sound that is not well suited for outdoor use. Major timbre issues were not noticed during use.

!!!info Summary of Tanchjim Bunny DSP impressions and EQ goals
- Bass is lacking "technicalities" due to a lack of sub bass
- Treble needs some lifting for outdoor use
- EQ will be used to improve bass quality and fix treble
!!!

***
## EQ

For bass, a peak filter at 20 Hz with a Q of 0.5 for sub bass. Moderate gain value of 5 dB was enough to improve bass "quality". However, bass is now dominating the whole sound, being a bit overwhelming. A small cut at 200 with a Q of 1 and -2 dB gain cleans up it up nicely.

For my own preference, treble will need to be slightly boosted; using **pink noise and music**, a small boost of 3 dB using a filter at 6 kHz with a Q of 1 helped a lot with clarity. **In my case**, any timbral issue or treble resonance problem was not significantly noticeable with outdoor use, except for a narrow peak around 11 to 12 kHz. Since this will be very different depending on the person, the filter for such use (fourth one) will not display any value. 

Compared to the Wan'er case study, the steps taken here are much simpler and shorter. Any measurement will do **as long as the conditions are the same** (very deep insertion in this case). The 5 filter limitation was also respected, with one remaining empty for any further FR refinement.

No picture will be provided as the changes did not rely much on measurements, and because the EQ was done using someone else's measurements. To visualize the changes, use an appropriate, deep insertion measurement of the Bunny. **Bold** filters are highly individual (ie only for me), and are excluded from the final FR; **every filter parameter should be modified to your preferences**. Preamp should be set to -5 dB.


Filter type | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|
PK | 20 | 5 | 0.5 | 
PK | 200 | -2 | 1 |
PK | 6000 | 3 | 1 |
**PK** | 11700 | -5 | 5 |
PK | X | X | X |


!!!
**Of course, this is just a small example and doesn't include a lot of what was discussed throughout the guide. From just these small judgments and steps, the sound has been improved considerably without having needed to spend more than an hour to come up with this preset. Further improvements can be had in terms of bass quality and treble refinement, but stopping here would be perfectly fine as well.**
!!!
