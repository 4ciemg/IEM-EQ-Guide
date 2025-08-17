---
order: 98
---
# Custom EQ presets to targets (\*)
While AutoEQ is excellent at what it sets out to do, it is also possible to EQ to a target manually. Results will probably be very similar to AutoEQ, but creating the preset allows for possible customization filters, and in cases where concise EQ presets are needed (eg when wanting to input presets on other apps/devices), AutoEQ can be non-ideal.

The best way to go about this is through squig in the Equalizer tab. Unfortunately, there aren't any direct steps to making a custom preset. Choose an IEM model, a target, and try to match the IEM FR as close as possible. Also try to include filters that can be customized easily to fit your preferences. For example, adding a bass/low-shelf is useful for adjusting bass levels on the fly by simply changing the gain and/or frequency. The same can be done with a treble/high-shelf, or even peak filters.

!!!warning
This is **a learning phase** and will not necessarily produce better results than AutoEQ. What it does produce is a better understanding of EQ, which will be useful later.
!!!

Here is an example of the difference between AutoEQ and manual EQ when it comes to using EQ on a model (in this case the Salnotes Zero 2) to a target (HarmanIE 2019, ignore the "adjusted"). At this stage, normalization has to be factored in, which can be done through a specific frequency (eg normalizing at 1kHz will shift every FR up/down such that the loudness) or with loudness based on equal-loudness contours. For the image below, AutoEQ filter values are on the left, manual EQ on the right. 
 
![AutoEQ vs manual EQ](https://i.postimg.cc/NMp0VHHW/Zero2.png)

Filter type | Frequency (Hz) | Gain (dB) | Q | Filter type | Frequency (Hz) | Gain (dB) | Q |
:-:|:-:|:-:|:-:|:-:|:-:|:-:|:-:|
 PK | 23 | -2.4 | 1 | PK | 150 | -3 | 0.5 | 
 PK | 120 | 0.6 | 1.3 | PK | 1800 | -1.5 | 1.5 | 
 PK | 130 | -3.1 | 0.5 | PK | 5800 | 5.5 | 1.5 |
 PK | 300 | -0.5 | 1.4 |  | |  | |
 PK | 890 | 0.7 | 2 |  |  |  |  | 
 PK | 1700 | -1.6 | 1.2 |  |  |  |  |
 PK | 6300 | 4.3 | 0.9 |  |  |  |  | 
 PK | 6500 |  3.5 | 2 |  |  |  | |
 PK | 7700 | -5.7 | 2 |  |  |  | |

AutoEQ uses every filter that is provided to it; if there are 9 filters available in the Equalizer tab in a squig.link database, AutoEQ will use those 9 filters to make the IEM FR as close as possible to the target. This also means that there are usually a lot of "useless" filters, like the one at 300Hz that has a very low gain with a relatively high Q value. In squig databases, it is possible to reduce the number of filters, but it is not something that other AutoEQ implementation can necessarily do; when comparing to the manual EQ preset, there is a significant reduction in the number of filters. Even if two customization filters were added (a bass shelf and a treble shelf), it would still be much less than the AutoEQ preset.



Pros | Cons | 
:-:|:-:|
Customization available | Not straightforward |
Better understanding of EQ | More time consuming than just using AutoEQ |
| | Not necessarily better sounding or more efficient than AutoEQ |
