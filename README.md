## REAKTOR 8STEPS Sequencer TouchOSC templates

### Description
This repository contains a collection of Reaktor 8STEPS Sequencer TouchOSC templates, to use for your music production setup. The purpose is to improve your workflow and inspire your productions.  

This tool uses your tablet like a "physical" tactile sequencer instrument to play virtual instruments hosted in your DAW, or external synths and modular gear. 

The role of the TouchOSC template is a midi controller, whereas the role of the Reaktor 8STEPS intrument is as a virtual sequencer "engine". The template sends the transport signals (play, stop, bpm), configure and play the sequencer values (pitch, gate, velocity, gate rate, gate lenght, steps, direction, offset, transpose, reset). The "sequencer engine" then responds accordingly sending the midi sequence to the instruments, and returning to the template the messages to display the position steps to provide a visual interactive experience. 

### Releases
| Version | Release | Description   |
| ------------ | ------------ | ------------ |
| ![Static Badge](https://img.shields.io/badge/1-green) | :link: [1.11.01](Reaktor-8STEPS-V1/) | Reaktor 8Steps Sequencer, 1 track, 8 steps, midi out, Ableton DAW-Hosted operation|
| ![Static Badge](https://img.shields.io/badge/2-red) | ![Static Badge](https://img.shields.io/badge/Development-red) |  Reaktor 8Steps Sequencer, 1 track, 8 steps, midi out, Standalone/DAW-Hosted operation, enhancements |
| ![Static Badge](https://img.shields.io/badge/3-red) | ![Static Badge](https://img.shields.io/badge/Development-red) |  Reaktor 8Steps Sequencer, 3 track, 8steps, midi / CV out, Standalone operation, 4 snapshots |


### [Version 1](/Reaktor-8STEPS-V1/) 
![Static Badge](https://img.shields.io/badge/released-green)
- Operation mode: Hosted in Ableton DAW
- 1 track, 8 STEPS, 1 MIDI channel
- 6 sequencer direction modes
- Clock: Ableton link
- MIDI mapping to Ableton device 	

<div align="center"> 

![](images/img1.jpg)

</div>

### Next Versions
Next versions will gradually extend the core funcionality and add more features.

#### Version 2
- 2 operation modes: a) Hosted in DAW, b)Standalone
- 1 track, 8 STEPS, 1 MIDI channel
- Position control enhancements
- Direction, Step, Offset radial controls enhancements
- OSC mapping control to Reaktor rack 	
- Keyboard template for Pitch tracking (transpose)
- 2 clock operation modes: Internal, Ableton link

#### Version 3
- 1 Operation mode: Standalone, 3 MIDI Channels
- 3 Tracks , 8 STEPS per track 
- Pause, Mute, link controls 
- 3 clock operation modes: Internal, Ableton link, External Sync clock
- MIDI Scales
- MIDI and CV output
- 4 Snapshots
- 3 clock operation modes: Internal, Ableton link, External Sync clock

### Support the Author
<p> 
I'm passionate about creating code that brings joy, inspiration, and creativity into people's lives. If you've enjoyed what I share and want to support my work, your contribution will help me to continue building. Every little bit fuels my creativity.
</p>

**_Thank you for your kindness and support!_** 

<a href="https://www.buymeacoffee.com/r1c4rd0" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

