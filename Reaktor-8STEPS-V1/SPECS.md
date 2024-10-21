
# Reaktor Bento Box 8STEPS Sequencer 

## Specification

--- 

### Version	
- Name: BB-SEQ1x8M Sequencer
- Version: 1.0 
- Release: 1.11.01 (240503)
- Author: Ricardo Acuña

---

### Sequencer
- Instrument: Reaktor Bento Box 8STEPS
- Tracks: 1 track 
- Steps: 8 steps  melodic sequencer
- Note Control: Pitch, Glide, Gate and Velocity
- 6 Sequencer control directions: 
	- fwd > 
	- rev < 
	- fwd-rev (Pendulum) <>
	- ping-pong <<>> 
	- brownian (semi-random) ?
	- random ?!
- Offset to define the initial position of sequence
- Reset position
- Pitch track (transpose) control
- Midi output: pitch and gate with velocity level
- External Ableton Link clock control
- Reaktor Preset file: 8-STEPS-1.11_.nksr
<br>

### TouchOSC	
- Template file: Reaktor-8STEPS-1.11.01.tosc
- Connections: MIDI, OSC, Bridge
<br>

### Integration
- Host: Ableton Live
- Remote control: MIDI and OSC protocol
- TouchOSC MIDI mapping to: Ableton Device, Transport (BPM, Play, Stop)
- Clock: Ableton Link
- Operation Mode:  Reaktor rack file hosted in Ableton
- Ableton template file: Reaktor-8-STEPS-1.11.als
<br>

### Requirements
- Platform: Reaktor 6
- Reaktor blocks: BLOCKS BASE
- DAW: Ableton Live 11+
- Control Surface: TouchOSC
- Mobile device: iOS iPad, Android Tablet
<br>

### Support the Author:
<p> Do you like it?, please support the author to continue development. <br>
Supporting means a lot to me, this will help me to continue building. <p>
<a href="https://www.buymeacoffee.com/r1c4rd0" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee" style="height: 41px !important;width: 174px !important;box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;-webkit-box-shadow: 0px 3px 2px 0px rgba(190, 190, 190, 0.5) !important;" ></a>

---

<br>

### Roadmap:

#### Version 2:
- Position control enhancements
- Direction, Step, Offset radial controls enhancements
- OSC mapping control to Reaktor rack 	
- No use of Ableton Live template
- Keyboard included in the template for Pitch tracking (transpose)

#### Version 3:
- 3 Tracks Sequencer
- Standalone operation (no DAW hosted)
- MIDI and CV output
- 4 Snapshots
