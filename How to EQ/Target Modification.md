---
order: 96
---
# Target Modification (\*\*)

Assuming that you're now familiar with EQ, it's time to dive a bit deeper into personal preferences. One good starting point is with targets, which have been tested and shown to be preferred by people. However, it has also been shown that while people do like specific targets, many also prefer some deviations from these. 

There have been several targets and FR curves that have been developed throughout the years, some with more validity and rigorous testing than others. For the sake of brevity, only popular and popular targets will be discussed here, but more can be found in the [Rigs, Curves, & Targets](https://4ciemg.github.io/IEM-EQ-Guide/rigs-curves-targets/) section. There are currently two targets that are used and recognized widely: the [Harman In-ear Target](https://4ciemg.github.io/IEM-EQ-Guide/rigs-curves-targets/#harman-in-ear-target-711--5128), and the [JM-1 Curve](https://4ciemg.github.io/IEM-EQ-Guide/rigs-curves-targets/#%CE%B4-and-jm-1-curve-711--5128). 

There are a few modifications that are worth trying out as studies have shown that listeners like varying levels of bass and treble. Furthermore, 

## HarmanIE 2019v2

The HarmanIE 2019v2 target is often used to gauge preference for IEMs, and while it it consistently rated very highly in preference testing, some resistance and criticism of the target have been present for as long as the target has been around. There are mainly two complaints about the target that exacerbate one another, and a minor one.

!!!warning Common criticisms of HarmanIE 2019v2
- The dip in the region around 200 Hz removes too much bass and warmth from the FR, leading to a thin sound.
- The ear gain region from 3 to 8 kHz is too elevated, leading to a shouty and overly bright sound.
- The treble dives down past 13 kHz.
!!!

Knowing these issues, the following filters were added. The left ones address the first two criticisms, while the two right ones are for preference adjustments for bass and treble. **Experiment and play around with the different frequency and Q factor values**.
Filter type | Frequency (Hz) | Q | Filter type | Frequency (Hz) | Q |
:-:|:-:|:-:|:-:|:-:|:-:|
 PK | 250 | 1 | LSQ | 100 | 0.71 |
 PK | 6500 | 1 | HSQ | 10000 | -1.5 | 
 
