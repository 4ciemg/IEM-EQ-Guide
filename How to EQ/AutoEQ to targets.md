---
order: 99
---
# AutoEQ to targets ( )

!!!info
The simplest way to use EQ is by using AutoEQ, a project that aims to create automatic EQ presets using measurements and a specific target. There are various implementations of AutoEQ: in most cases, AutoEQ aims for the HarmanIE 2019 target. The following sections cover most cases, and also have pros/cons added.
AutoEQ has a wiki that explains how it functions, but in short, it aims to match the FR of a model to a chosen target in the range of 20Hz to 10kHz. For the guide, both the lower and upper limits will be used.
!!!


## AutoEQ website
AutoEQ.app is a web application for the AutoEQ project, and has additional features for further tweaking and customization. 

1. Find your IEM model
2. Select the EQ app you plan on using
	2*. Under the Advanced option in the Profiles tab, select your target of choice
3. Download the file
4. Import/use the file in your EQ app of choice.


Pros | Cons | 
:-:|:-:|
Live demo'ing | Somewhat overwhelming/convoluted at first |
Customization available | Customization can lead to bad results |
Wide EQ app support | Somewhat limited model selection |



***
## EQ app 
Several EQ apps have also implemented the AutoEQ project, such as Poweramp on Android and PeaceGUI on Windows. In this case, simply pick the IEM model you have and the preset should apply automatically.

1. Find your IEM model and apply the preset

Pros | Cons | 
:-:|:-:|
Easy to use  | Somewhat limited model selection |
No additional installation |  |


***
## Squigs
Squig databases also have an Equalizer tab that implements AutoEQ. To use it, select the target that you want (under the FR graph), then select your IEM model in the Models tab, ensuring that only the chosen target and IEM are on the FR graph. In the Equalizer tab, find the AutoEQ option, adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project), generate the preset, then export it accordingly.

1. Select the wanted target under the FR graph
2. Select the IEM model in the Models tab, ensuring that only the chosen target and IEM are on the FR graph
3. Find the AutoEQ option in the Equalizer tab
4. Adjust the range (maximum upper limit around 10kHz as specified by the AutoEQ project)
5. Generate the preset
6. Export the preset accordingly

Pros | Cons | 
:-:|:-:|
Extensive selection of models and targets | Export only exports the filter values which need to be manually re-input in whatever EQ app is being used |
Customization available | Default range extends to 15kHz, far above what is recommended |
| | Can be inefficient since it only uses peak filters

***
## Wavelet
Wavelet is an Android app that has AutoEQ implementation and allows for system-wide equalization. 

1. Enable Wavelet
2. Choose your IEM model in the AutoEQ section
	2*. If needed, import presets made in squig.link or AutoEQ.app


Pros | Cons | 
:-:|:-:|
Easy to install and use  | No customization possible |
Presets available from other sources | Hassle when making a new preset |


