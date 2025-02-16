---
order: 96
---
# EQ to preference and context (\*\*)
Assuming that you're now familiar with EQ, it's time to dive into personal preference targets. While preference targets with small tweaks (eg an added bass or treble shelf) are a good way to start, they might not be the optimal sound that each person is looking for, which is why having an understanding of one's preferences is crucial. 

At this stage, the possibilities are endless which also means that everything can become overwhelming. What should be modified first? What if it doesn't sound good? What if X or Y is a mistake? 

Now that you are hopefully more familiar with your preferences as well as EQ, let's add a few rules and important notes.

!!!warning More rules 
- FR should be interpreted holistically where changes in one range can impart perceptual changes in another.
- Changes in on frequency range (eg bass) can be perceived as either a direct change in the targeted region, or a change everywhere else
	- Eg. a reduction in bass can be thought of as just that, or as a boost everywhere else except the bass region
- Human hearing is more sensitive to peaks than dips in FR
- The debate between accuracy and enjoyment should be ignored in favor of what sounds good to you
- Listening tests are **necessary**. Overreliance on graphs can lead to bad results
- Experiment with the filter types and parameters while still adhering to EQ minimalism to achieve different results
!!!

There are two aspects to consider: preference and context. Preference as described above might not match a specific target, and should therefore be **explored through experimentation**. Context refers to everything from the audio to the listening environment and how the IEM is being used. Factors to consider for both are numerous, such music library which can have inconsistent mixing and mastering between different genres, releases, discographies, and even within the same project, and environmental noise, which might necessitate more volume for certain frequency ranges. 

!!!info Let's divide the frequency range into three distinct regions
1. Bass 
	- Sub bass (20Hz - 80Hz)
	- Mid bass (80Hz - 300Hz)
2. Mid range
	- Lower mids (300Hz - 1kHz)
	- Upper mids (1kHz - 4kHz)
3. Treble 
	- Treble (4kHz - 10kHz)
	- Upper treble (10kHz - 20kHz)
!!!

***
## Bass
Fortunately for IEMs, bass output is usually not a problem provided there's a good seal between the canal and IEM. The differences in bass between different IEMs can be simplified to two aspects that can be tweaked to preference. 

!!!info Bass 
	- Bass level, which refers to the overall average bass response loudness relative to the rest of the response. It can be high, low, or anything in between
	- Bass shape, which refers to the relative balance between sub and mid bass. Useful for different bass "presentations"
		1. Bass glide: Generally refers to bass that has a "good balance" between sub and mid bass. Can be a a straight line as shown, or more contoured
		2. Flat bass: Equal levels of sub and mid bass
		3. "Subwoofer" / Tucked bass: Heavy emphasis on sub bass, with much lower relative mid bass level
		4. Rolled off: Emphasis on mid bass, with sub bass levels that are decreasing and lower than mid bass
!!!

The following pic shows the different bass shapes in order. Note that this is just a very small sample of what bass can look like on IEMs. The number of variations and small tweaks that are possible can also muddy the waters and create differently perceived bass presentations despite looking mostly similar on graphs.

![Different bass shapes (in order and normalized at 1kHz)](https://i.postimg.cc/Pq9fBdpX/Bass.png)

Bass is the most variable range in terms of preference, so experimenting with not only different shapes but also levels is really important. Bass is also highly variable depending on the audio signal / music you're listening to. For example, acoustic-oriented music will not have as much bass as hip hop, or electronic music. The goal is to find the right balance between your preference and what you're listening to. 

!!!warning EQ based on genres
Whether EQ should be suited to match one's library or simply used to correct the IEM's FR has been debated ad nauseam. For this guide, do whatever suits you in terms of accessibility, ease of use, and sound preference.
!!!

***
## Mid range
Mid range is a tough region to tweak because it is wide in range and also contains a lot of the audio content. Most if not all instruments and components in music have some part of their frequency content in the mid range: everything from bass instruments to high pitched percussions are therefore affected by changes in the mid range. As with bass, mid range can be simplified into three aspects.


!!!info Mid range
- Ear gain elevation, which refers to how high/low the ear gain is **relative to the rest of the response**
- Ear gain location, which refers to where the maximum peak of the ear gain is situated at. Common location is at 3kHz
- Mid range shape, which refers to the relative balance between lower and upper mids. Useful for changing note weight / brightness / warmth / etc.
	1. Recessed mids: Low levels of lower mids, leading to the mid range sounding "thin" and "hollow"
	2. Forward mids: **Usually** refers to high levels of upper mids and/or ear gain.
	3. Low ear gain: Low levels of mids, usually above 1kHz, relative to the rest of the response
	4. Warm/thick mids: High levels of lower mids, leading to a more "full-bodied" mid range and more "warmth".
!!!

Mid range has a lot of variation between different IEMs, so much so that it becomes rather hard to demonstrate these different aspects independently. Aiming for a similar mid range as ones found in preference targets should be the goal, but don't be afraid to make big changes if it sounds better to you. The following pics shows different mid range responses and how variable they can also be. Also notice how different normalization can skew visual perception of mid range, which is why listening to the EQ changes is recommended.

![Different mid range responses (normalized at 1kHz)](https://i.postimg.cc/VvV30YxS/mids-1khz.png){width=400} ![Different mid range responses (normalized at 300Hz)](https://i.postimg.cc/WpYRHnd2/mids-300hz.png)


***
## Treble
Treble is the trickiest and most difficult region to tweak because of measurement variance, insertion depth, HRTF differences, and more. At this stage, only two aspects are considered.

!!!info Treble
	- Treble level, which refers to the level of treble relative to the rest of the response
	- Treble peaky-ness, which refers to the presence and/or absence of large, noticeable peaks
!!!

Doing any changes in treble should, in most cases, only rely on listening tests and not graphs. If there is a treble flaw attributable to the IEM, only then should EQ be considered. For now, treble modifications should optimally only involve shelf filters and/or low-Q/wide peak filters to change treble and upper treble levels. Depending on taste and the IEM's FR, boosting or reducing with these filters should improve overall tonal balance without much effort. 

In the case where there is an obvious peak that is sibilant and/or annoying, there are a few steps to take.

!!!info Fixing treble peaks
1. Confirm that a peak is actually present in the IEM's FR and that it is not a peak that is present in the audio content
2. Determine whether or not this peak has a noticeable, negative impact; continue if it does
3. Locate the peak using music, pink noise, or a tone generator / sine sweep. A tone generator/sweep can also work, but should be done even **more critically as human hearing is not good at detecting perceived loudness** with sine signals. **Only use it for very high amplitude peaks**
4. Use a relatively sharp filter (Q > 4) and varying levels of negative gain, ensuring that the peak is minimized without encroaching on the surrounding frequency range (ie reduced until no longer bothersome) by using music and/or pink noise
!!!

***
## Adding everything together
As mentioned previously, FR should be interpreted holistically. It is therefore wrong to think that because two IEMs have the same bass response, they will sound the same in terms of bass. Every single region affects one another, and it is hard to completely separate each region, especially when it comes music. It is therefore important to test in various ways. Keeping two regions locked and modifying one is a logical approach, but locking one and modifying the other two regions can also lead to interesting and unexpected results. Mix and match and try to experience many different FRs.

!!!warning
Listening to each frequency region independently does not reflect how music is heard. Changes in FR should be done with the knowledge that any change in any of the regions will also affect the perception of the rest of the response. At this stage, **experiment and try everything you can**.
!!!

In the end, the final obtained FR should be ideal to your preferences, and while large deviations in bass and treble regions are normal, the mid range should still have a generally "normal" profile (ie have some semblance of ear gain). The following collection of images are some commonly seen and liked "types" of FR with small descriptions of their tuning; use them as a template and/or mix and match different parts. 

||| === Common ear gain with a bass boost (glide) 	
    ![](https://i.postimg.cc/NFhCkjQZ/zero2.png)

![Forward mids and ear gain with bass boost; emphasis on mid bass by rolling off the sub bass](https://i.postimg.cc/8zT3YcLS/Origin.png)
![Somewhat flat or rolled off bass with a lot of lower mids (warmth), with low plateau ear gain](https://i.postimg.cc/KYHH45wG/Andro.png)
||| ![](https://i.postimg.cc/NjbVvtxr/Proxima.png)
![Sub bass boost followed by a mid bass dip with forward ear gain](https://i.postimg.cc/bJSFntfQ/Variations.png)
![Bass boost (glide) with moderate plateau ear gain](https://i.postimg.cc/5NBTpLYg/P5.png)
||| ![Sub bass boost with very little to no ear gain](https://i.postimg.cc/15hbpJt4/MEST2.png)
![Bass boost (glide) with low ear gain except for a 4.5kHz peak](https://i.postimg.cc/FFJ2d2h2/CRA.png)
![Mostly sub bass boost with moderate ear gain](https://i.postimg.cc/Bv6zqzh7/5EST.png)
|||



=== Common ear gain with a bass boost (glide) 	
![](https://i.postimg.cc/NFhCkjQZ/zero2.png)




***
## Noise and environment
Depending on the listening environment, more changes might be useful. There are a lot of factors at play here, such as whether or not the IEM being used has ANC, what the listening volume is currently, what the noise attenuation profile of the IEM is, how loud the surroundings are, if there's a need to be aware of voices or signals, etc. Ultimately, correcting for these factors requires experimentation just like what was discussed previously. A few rules can be used.

!!!info Tips and common scenarios
- Research suggests that in loud environments, a boost in bass is preferred. Most probably depends on the its noise attenuation profile
- Based on equal-loudness contours, EQ might need to be adjusted to suit a specific listening volume
- Good ANC will cancel out bass more effectively than passive isolation, but will also struggle with frequencies above 1kHz
!!!
