---
order: 93
---
# More advanced DSP (\*\*\*\*)
Digital signal processor (DSP) refers to, in this context, to any software/tool that changes the signal, in this case being audio. EQ is a form DSP, but there are many other ones that can change the audio signal in ways that EQ can't. This section will cover some common forms of DSP, as well as some more niche ones. At this stage, there won't necessarily be any improvement in sound; it is yet another experimentation stage. Whether or not you prefer them or regular stereo music will depend on your preferences.

A lot of DSP will be applied through **convolution** (with .flac or .wav files) and/or **VST plugins**, both of which are supported in EqualizerAPO through the "Editor"/"Configuration Editor" app (comes with EqualizerAPO). The explanations will also be brief and only cover the essentials. 

***
## Crossfeed
When listening to loudspeakers, the signal out of one channel will still reach the opposite ear; with IEMs, there is a lack of such an event. Crossfeed fixes this issue by feeding a "small" signal of each channel into the other. It might seem like crossfeed is a necessary and obvious tool that would result in a consistently better preferred sound, it is definitely not as simple as it seems. For hard panned music (eg early jazz recordings with bass in one channel and the other instruments in the other one), crossfeed can help with creating a more cohesive sound presentation. However, most music uses "soft" panning, where the positioning of elements isn't as extreme; crossfeed is indirectly being applied here. It is therefore important to test with crossfeed to see if the change is actually preferred or not. Crossfeed implementation can vary in terms of theory, implementation, customizability, and more, all of which are beyond the scope of this guide. **A few common ones include BS2B, Chu Moy, and Jan Meier crossfeed**.

***
## Dynamic EQ
Dynamic EQ adds another variable into play, which is the incoming signal (in this case being the music); when the signal/music in the specified band passes a loudness threshold, the filter "turns on". Compared to regular/static EQ, the change is **not applied throughout the whole track**. Using it can add another layer of finetuning as it allows for more precise and less disruptive filters. For example, if there's a part in the track that has a substantial amount of sibilance, a regular EQ filter can be used to cut that out, but this also cuts everything including other elements in a track. Using a dynamic EQ, the threshold can be set such that only the loud sibilance triggers the filter while the rest of the track is unaffected. This method is also applicable for improving bass response while minimizing excess lower mid levels. 

While the benefits can be worthwhile, it is important to note that any dynamic EQ presets will **have to be checked and modified depending on the music**. The main difference between regular EQ and this dynamic EQ is that the former focuses on modifying the IEM's FR while only slightly considering music; the latter is more related to the music itself, for which the spectral information can change drastically depending on the genre, mastering, release date, and more, which will **inevitably lead to needed modifications in the dynamic EQ preset**. 

***
## Distortion, compression, and others
Many effects used in the music production side can be applied in this context as well. Distortion might be preferred for some, so adding a bit of distortion and experimenting with different distortion implementations can be effective without having to rely on external devices. The same applies to compression in cases where dynamic range is too high, track mixing isn't up to preference, or for any other reason. A slight delay between channels can also result in a preferred sound presentation. There is a wealth of softwares and DSPs that can change the incoming signal in simple ways like what has been discussed here, or in more extreme ways.


***
## HeSuVi and HRTFs
[HeSuVi](https://sourceforge.net/projects/hesuvi/) is a program that utilizes EqualizerAPO's convolution filter to imitate surround sound (5.1/7.1/binaural sound effects) virtualizations for headphones/IEMs. Included with the software are Head related impulse responses (HRIRs), which can be thought of as recordings of a loudspeaker's response at a specific direction measured with "head mics" (ie measured response at the eardrum). With multiple HRIRs in different directions, it becomes possible to simulate "virtual loudspeakers" for 5.1/7.1 surround sound virtualization. It therefore becomes possible to listen to 5.1/7.1 recordings without an actual surround sound system; while an interesting proposal, the lack of such recording makes it a niche product. The interesting part comes with adding said HRIRs with stereo recordings, in which case an added level of "spaciousness".

The quality of the HRIR varies greatly, and changes depending on how it was made and the intended goal. On the right side, there are common HRIRs, usually from other popular implementations of surround sound virtualization (mainly gaming related), and on the left side, other HRIRs from various databases. The [Binaural Audio](https://binaural-audio.slite.page/p/i38zsD7728/Binaural-Audio) and its corresponding [Binaural HRTF Database](https://airtable.com/appayGNkn3nSuXkaz/shruimhjdSakUPg2m/tbloLjoZKWJDnLtTc)  are resources that contains many different HRTFs/HRIRs and can be useful for quick testing in order to find a good fit.

![HeSuVi](https://a.fsdn.com/con/app/proj/hesuvi/screenshots/HeSuVi_Virtualization.png/max/max/1){width=600}

***
## HRTF Creation and room virtualization/simulation
Proper HRTF measurements are not feasible for most people, and are usually only conducted for population studies or done with mannequins. Companies like Apple and Final Audio employ different methods to account for HRTF, such as taking quick 3D scans of the ear, or by measuring the canal entrance response with microphones in and around the IEM. However, these solutions are either restricted to their own ecosystem, or are limited in accessibility.  There are however a few projects that try to bridge this gap by offering relatively simpler methods of acquiring said data, although their effectiveness is not ideal and effectiveness remains to be seen. 

[EAC - Individualized HRTF synthesis](https://github.com/davircarvalho/Individualized_HRTF_Synthesis) is a project that uses ML to recreate an HRTF measurement based on real-life measurements of the ear. The process requires the user to take measurements of their ear - there is a tool to facilitate the task using pictures and a reference length - and inputting them into their software. The final result is an HRTF SOFA file that can be used in room virtualization software. The HRTF file itself is not particularly useful; it needs another program, usually one that attempts to simulate a room with said file. For example, with their HRTF SOFA file, the user can then use another program that simulates a room to the user's need, and for which the response of the person's HRTF can be had. It is therefore possible to recreate a room that has a diffuse sound field, incorporate the HRTF, and measure the DF HRTF of the user. The author of the paper also has several other projects, such as a Webcam Head Tracker and a Room Auralization, with the latter being able to use SOFA HRTFs.

The issue with this method is that the synthesized HRTF itself deviated significantly from their actual acoustically measured HRTFs. There is also the lack of ear canal geometry, head/torso dimensions, and finer ear details in the HRTF calculations; all of these factors can lead to synthesized HRTFs that aren't ideal. The deviations shown in the image below highlight the large differences in amplitude between the proposed/synthesized response (dotted lines) and the original/measured response (solid lines) as well as the overall smoothed result.


![Comparison between synthesized and measured HRTFs on the horizontal plane at various azimuths](https://i.postimg.cc/6px0Gksz/EACsynthesis-HRTF.png)


[MESH2HRTF](https://www.mesh2hrtf.org/) is an open-sourced project that uses the same concept as the previous project, except it requires a 3D scan of the whole ear and head. The mesh is then used with modeling software like Blender and the project's own calculator to obtain HRTFs for specified angles in a free-field. It is also possible to obtain a SOFA file for the HRTF and to use it in other room simulation softwares. The accessibility of this project is rather low, requiring at the very minimum a modern iPhone which will produce less than ideal results, or a professional 3D scanner. Furthermore, the same problem of not accounting for canal geometry still applies here.

![Mesh2HRTF](https://raw.githubusercontent.com/Any2HRTF/Mesh2HRTF/master/docs/figures/graphical_abstract-01.png)

For room simulation, there are a few projects that have SOFA implementation. [Anaglyph](http://anaglyph.dalembert.upmc.fr/) and [SofaMyRoom](https://robaru.github.io/sofamyroom/) are both programs that allow for localization customization based on various parameters; Anaglyph is focused on ILD and ITD changes with simplified localization modifiers, while SofaMyRoom is focused on room emulation with different room and loudspeaker parameters. As mentioned previously, there is also the [Auralization Engine](https://github.com/davircarvalho/Auralization_Engine) project that aims to create virtual audio scenes; this program only works with one track at a time, but is worth taking a look at as it includes head tracking and is relatively accessible.

+++ Auralization engine
![](https://raw.githubusercontent.com/davircarvalho/Auralization_Engine/master/Images/1.PNG)
+++ Anaglyph
![](https://i.postimg.cc/cC3B6SmR/Anaglyph.jpg)
+++

***
## Custom DSP
It is of course possible to create your own DSP if any of the current offerings are not enough. EqualizerAPO itself is a very powerful tool that allows for a lot of customization and signal mapping/processing, and combined with its convolution filter, it is overall an excellent method of experimenting. Both this method as well as creating a DSP is way beyond the scope of this guide, and should only be attempted by the curious. Most solutions are already available for way less effort.
