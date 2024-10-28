## Reaktor 8 STEPS Sequencer
### Version 1.2
- Reaktor 8 STEPS Sequencer, 1 track, 8 steps, MIDI, Hosted
- Model:    SEQ-8S-1T8S-MH
- Version:  1.2
- Release:  1.2.0
- Author:   Ricardo Acuna
- Date:     2024-oct-27


<div align="center"> 

<img src="images/img3.gif" >

</div>


## Description
A basic and easy to use TouchOSC template to control a Reaktor 8 STEPS Sequencer virtual instrument. It can be used in a simple setup to improvise in your workflow, enjoy and inspire your productions. The template sends the transport signals (play, stop, bpm) and sequencer values (pitch, gate, velocity, gate rate, gate length, steps, direction, offset, transpose, reset). The sequencer sends the midi sequence to other hosted instruments in your DAW.  A return track in your DAW sends back the midi messages to visualize the position steps for an interactive experience. It materializes a small and basic "physical" sequencer for your musical production workflow to play any Ableton virtual instruments or even an external modular gear by using it with Ableton CV tools.

<div align="center"> 

<img src="images/img1.jpg" >

</div>

<br>

## Contents
- [Instrument](#instrument)
- [Sequencer](#sequencer)
- [Connections](#connections)
- [Requirements](#requirements)
- [Files](#files)
- [License](#license)
- [Support the Author](#support-the-author)


## Instrument
- Plugin: Native Instruments Reaktor 6 
- Library: Blocks Base
- Main Module: SEQ-Bento 8 Steps Sequencer
- Operation Mode:  **hosted** in Ableton Live
- DAW Host:  Ableton Live 11/12

## Sequencer
- Modular Block: Reaktor Bento Box 8 STEPS
- Tracks: 1 track 
- Steps: 8 steps, melodic sequencer
- MIDI out: Pitch, gate (with velocity level)
- Modulation: Velocity, Gate time, Glide
- 6 Sequencer directions: 
	- fwd > 
	- rev < 
	- fwd-rev (Pendulum) <>
	- ping-pong <<>> 
	- brownian (semi-random) ?
	- random (full-random) ?!
- Offset: initial position of sequence
- Reset: reset to initial position 
- Pitch track: transpose using an external midi controler
- Clock: External, Ableton Link 
- MIDI CC out: CC101 (gate), CC102 (position), CC103 (play)

## Connections
- Reaktor Mapping: OSC
- Ableton Host Mapping:  MIDI
- Connections: MIDI <Bridge1>
- Connections: OSC Host, Ports: send 10000, receive 10000
- Bridge: IP of your PC host
- Setup: 
	- Bridge: setup IP of your PC host
	- OSC: setup IP of your PC host
	- Ableton Live settings: TouchOSC Bridge Input Port (Track, Remote), Output Port (Track, Sync, Remote)

## Requirements
- Control surface software: TouchOSC
- Tablet: An iOS or Android Tablet
- DAW: Ableton Live Version 11 or 12
- Plugin: Native Instruments Reaktor 6 plugin with 
- Reaktor Modular Blocks: Blocks Base
- MIDI controller: Optional for external pitch transpose
- Target virtual instrument: Any virtual instrument in your DAW
- Target external instrument:  Any external midi instrument using midi out or Ableton CV tools (optional)

### Files
- TouchOSC Template: SEQ-8S-1T8S-MH-1.2.tosc
- Reaktor Rack:      SEQ-8S-1T8S-MH-1.2.nksr
- Ableton Live set:  SEQ-8S-1T8S-MH-1.2.als
	- Track 1 - Reaktor sequencer: contains the Reaktor 8STEPS rack (preset), MIDI input receives transpose, MIDI out sends to track 2 and track 3.
	- Track 2 - TouchOSC Bridge MIDI return: receives CC´s from track 1 and sends back to the template, TouchOSC Bridge MIDI out. 
	- Track 3 - Basic Square: A sample Ableton stock virtual instrument, MIDI input from track 1. 

<div align="center"> 

<img src="images/img2.jpg" >

</div>

## License
![GitHub License](https://img.shields.io/github/license/murry61/touchosc-reaktor-8steps)
All assets and code are under the MIT LICENSE in the public domain unless specified otherwise.


## Support the Author
<p> 
I'm passionate about creating code that brings joy, inspiration, and creativity into people's lives. If you've enjoyed what I share and want to support my work, your contribution will help me to continue building. Every little bit fuels my creativity.
</p>

**_Thank you for your kindness and support!_** 

<a href="https://www.buymeacoffee.com/r1c4rd0" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>
