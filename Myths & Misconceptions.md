---
order: 94
icon: alert
---

# Myths & Misconceptions

!!!warning
WIP
!!!

!!!
The following section covers a few myths and misconceptions that are popular, and whether or not they have any validity.
!!!


## More than Frequency Response?
The first thing to consider is whether or not FR is the only measurement that should be looked at, as EQ and the guide are based on the concept of FR being the dominant aspect of sound quality. In fact, the EQ guide works on the premise of IEMs being minimum phase systems for which the FR can be changed using minimum phase filters (used in most EQ software). The following sub sections cover different measurement types and their importance when assessing sound quality and EQ.

### Distortion/Nonlinearity
The most obvious measurement to look at is distortion/nonlinearity. In the case of IEMs which are low excursion transducers, nonlinearity is mostly characterized by harmonic distortion (HD), and therefore any increase in other distortion metrics will be reflected in HD. It is therefore common to see measurements of total harmonic distortion (THD) when distortion figures are provided along with the tested SPL level. Indeed, as the SPL output of an IEM increases, so does distortion; when using EQ, the preamp will reduce the digital volume, but most will also increase the volume a bit to counter the preamp. Therefore, any time a positive gain filter is used in an EQ, the distortion in the affected region will increase.

What is not common is the inclusion of psychacoustic models such as masking. Therefore, most distortion measurements will be shown with two options: the first presented as "raw" data with no indication for how humans will perceive it, and the second with a generalized rule of thumb concerning distortion audibility. In both cases, the technical data is presented without much consideration for the human perceptual system. However, in **most cases, distortion will not be perceptually significant with IEMs**, and will not be audible **even with extensive EQ**. It is therefore unecessary to consider nonlinearity as being a big factor when using EQ.

### Transients, Speed, & Responsiveness
A transient is often explained as being a short duration, single instance sound, such as the pop of a balloon or a gunshot. These are usually displayed in the time domain; instead of having frequencies on the x-axis, it is instead time. 

The most common method way of seeing the transient response of IEMs (and other transducers) is by measuring the impulse response (IR). A single impulse is fed into the IEM, and the obtained output shows the response of the IEM over time. This single impulse contains all frequencies at the same amplitude, after which a Fourier transform of the IR is used to separate the frequencies and the corresponding amplitude of each frequency, which changed due to the FR of the IEM. **In fact, FR measurements are all done by first measuring the IR of the IEM, then doing the Fourier transform of it to obtain the FR.**

Below is a demonstration of the link between FR and IR shown with two IEMs; both were measured, and one was re-measured using EQ to approximate the other IEM within reason (+/- 0.5 dB). By using EQ, or any method of changing the FR, there is a corresponding change in the IR. **These are causally linked, and therefore contain the same information**. However, IR is not helpful when trying to correlate it with what is being heard, and **is not a valid method for characterizing "speed"**.

+++ Original FRs
![](https://i.postimg.cc/Gp1RCDv0/FR.jpg)
+++ Original IRs
![](https://i.postimg.cc/mD57cTLs/IR.jpg)
+++ Modified FRs
![](https://i.postimg.cc/L8PSwDYB/FR-2.jpg)
+++ Modified IRs
![](https://i.postimg.cc/RhJKK2hn/IR-2.jpg)
+++ Difference?
The small differences in the modified IRs are due to non-perfect matching of the two FRs. The modified FR graph even shows visible discrepancies between the two FRs, which then lead to different IRs. 
+++

***
## Tuning & Technicalities Dichotomy
Popularized by Crinacle and adopted by many, the tuning versus technicalities dichotomy has become the most common way of thinking about sound quality with relation to IEMs (and headphones). The prevalence of measurements combined with uncertainty and mismatch with perception has resulted in a split between "easy to explain" aspects, grouped under tuning for and in consequence FR, and "hard to correlate" aspects, grouped under technicalities. The latter is of importance, since it is often thought of as being separate from tuning and FR, when that is not the case; in fact, based on what has been discussed before, **FR is the most important metric for predicting sound quality and dominates over every other one**.

There are a few camps where most people reside in: 
It is therefore possible to modify these so-called technicalities with EQ once an understanding of FR is acquired. The following presents a few points of discussions.

!!!
- WIP
- WIP
- WIP
!!!


***
## Test Signals vs Music
Another common misconception involves the test signal used for measurmeents. Indeed, many argue that the sine sweep that is used currently is not representative of real-life "complex" signals like music, with many frequencies at different amplitudes occuring at the same time to the point where IEMs will have varying levels of "accuracy".

Depending on the algorithm, different stimulus signal can be the input, whether it be noise, music, sine sweep, etc. The resulting FR will always be the same (sometimes with miniscule differences). White noise, which contains all frequencies at the same amplitude, is similar in concept to IR with its single impulse containing all frequencies at the same amplitude. Music can be thought of as a form of noise, with the caveat of music having an FR of its own which will have to be removed by the algorithm in order to only obtain the transfer function of the IEM and not of both.

Nowadays, measurements use an exponentially-swept sine signal as detailed by Angelo Farina, which allows the user to measure both linear and nonlinear behavior of IEMs (or other DUTs) in a short time. In REW, options for measuring with sweeps and noise are available; a real-time analyzer (RTA) function is also present, allowing the user to measure the real-time response of an IEM (works best with white noise; if using music, the average FR of the music has to be subtracted).

***
## Driver Type & Configuration Differences
Similar to the tuning and technicalities dichotomy, there are also a lot of ideas and concepts related to the drivers themselves that have been created and perpetuated to explain various perceived sound characteristics, despite many of them being false. 

For driver type, perhaps influenced by similar thinking in the headphone hobby...


