## REAKTOR 8 STEPS SEQUENCER CONTROLLER - TouchOSC template

<div align="center"> 

![](images/img0.gif)

</div>


### Description

A Reaktor 8 STEPS Sequencer TouchOSC template to use it as an external sequencer midi surface controller for your musical production setup. With it you can use your hands-on to play and control a BLOCKS REAKTOR 8 STEPS sequencer for your virtual instruments in your Ableton DAW or even with an external modular instrument using Ableton CV tools. It follows the sequence steps on sync, lighting them and giving a visual and incredible interactive experience. The main motivation to design this template was to have a hands-on experience with the realization of a touch controller as a “physical” sequencer to play your virtual instruments or even your external modular gear in a hybrid setup. 

---

### Requirements

-   TouchOSC and TouchOSC Bridge
-   An iOS or Android Tablet
-   Ableton Live Version 11 or 12
-   Reaktor 6 (Player or Full), with Blocks Base
-   A MIDI controller for external pitch
-   A virtual instrument in your DAW
-   An external instrument with Ableton CV Instrument (optional)

---

### Setup and Configuration
The template is designed to work with Reaktor 6 ***HOSTED*** inside Ableton Live. You can use it to play a sequence either with virtual instrument (VST plugin) or with an external instrument (MIDI or CV Tools). An important consideration for the design was the use of Ableton Link to keep the clock synchronization of the sequencer steps with the TouchOSC controller. The following files are included in the repository to quickly setup and run it. The files contain all the midi and osc mappings required and the Reaktor 6 rack wiring. 

![](images/img3.Ableton_TouchOSC_setup.jpg)

| File | Description   |
| ------------ | ------------ |
|  [Reaktor 8STEPS - 1.11.tosc](touchosc/Reaktor-8STEPS-1.11.01.tosc) | The TouchOSC template to control the Reaktor Blocks 8 Steps Sequencer  |
| [Reaktor-8 STEPS-1.11.als](files/Reaktor-8-STEPS-1.11.als)   | Ableton Live Template   |
| [8-STEPS-1.11.nksr](files/8-STEPS-1.11_.nksr)  | Reaktor 6 - 8 Steps preset   |

Ableton Live provides midi feedback to the TouchOSC template using a [device control mapping](images/img4.Ableton_Reaktor_Device_Controller.jpg). This allows bidirectionality and automatic update of each control when you change it either in the TouchOSC template or in the Reaktor 6 plugin. The Ableton Live template has all the [midi mappings](images/img9. Ableton-MIDI-map.jpg) already configured. Ableton Live send and receives MIDI signals through [TouchOSC Bridge](images/img5.TouchOSC_Bridge_config.jpg). You need to setup it in Ableton Live with Track, Sync and the Remote-control options.

---

### Features

The template has all the functions of the BLOCKS REAKTOR 8 STEPS sequencer, an accurate reproduction of the original virtual instrument. Additionally, it follows the sequence steps on sync, lighting each step and giving a visual and interactive experience. The template scripts contain carefully crafted algorithms to match the sequencer steps progression with the gate and start/stop midi signals.  The complete wiring of the Reaktor rack preset is as follows: 

![](images/img6.Reaktor-8-STEPS-rack.jpg)

The template also includes additional controls to enhance the functionality:

- C3 button – to center all the steps to C3
- Manual Gate (diamond button) – to play a manual gate to easy adjust the pitch on each step. 
- Play button – To start the sequencer, synchronized with Ableton Link on the beat.
- Stop button - To stop the sequencer.
- Clock Gate button –Allows you to set the number of gates sent for every beat
- Clock Shuffle button – To add shuffle or swing.


Just two [OSC mappings](images/img7.Reaktor_OSC_map.jpg) are used in Reaktor, which are already configured in the Reaktor rack preset. The controller makes use of [arrows buttons](images/img8.Direction-Steps-Offset.png) to control the direction, steps and offset instead of the radial control directly. The reason was to prevent out-of-sync jumps when touching the radial controls that creates a bouncing effect on x values.

---

### Instructions

1. Load the TouchOSC template in your Tablet.
2. Check you have enabled and working the MIDI, OSC, and Bridge connections.
3. Configure in your tablet the OSC and Bridge connections with the host IP of your computer running TouchOSC Bridge. 
4. Load the Ableton Live set and the Reaktor preset files in your computer. 
5. Start the Ableton Live set. The first time, you would need to update the Reaktor preset location by selecting it from your file directory. Then save your live set. 
6. Enable Ableton Link
7. Check you have the TouchOSC Bridge configured in Ableton as required.
8. Check the MIDI/OSC connections are working as pictured in the setup diagram.
9. The first time you run the template try moving all the controls to pick-up the controls. 
10. Select a virtual instrument of your choice in another Ableton track (or an external instrument) and select Reaktor 6 as the MIDI input to receive the sequencer output. 
11. Configure your sequence as you wish: direction, steps, offset, velocity, glide, gate, gate rate, bpm and so on
12. You are ready to play. Enjoy!

---

#### Notes

<div align="center"> 
  
  <img src="images/img2.Reaktor-8STEPS_layout.png" with=500 height=500>

</div>

**PLAY**. Once you press the PLAY button your sequence start playing. You can change any parameter of the template while running as you wish. The template will keep on sync with the beat. 

**RESET**. Although the template controller is designed to keep on sync all the time, occasionally it could loose sync, depending on the connection’s latency and the CPU and tablet resources. Just press the RESET button and it will recover. This would probably happen when you select high gate rates 32th or 64th or high BPMs. 

**C3**. A C3 button is provided to center the pitch off all steps. This is useful when you are starting to set-up a new sequence from scratch.
Manual Gate. A diamond shaped button is provided to trigger a manual gate to move one step. This is useful when you are starting to set-up a new sequence from scratch to test the sequence.

**GATE**. Internally the gate control is limited to 100 (not 127), to prevent overlapping of notes that could produce loose of sync. 

**GLIDE**. The glide control produces slides to the pitch of the following played note, creating a “portamento” or “glissando” effect. Take care, it could produce out of scale notes.

**MIDI OUT CC 101**. This is an important midi signal that the template uses for gate control. Do not unintentionally unwire it, to prevent your template to fail. 

**RACK PRESET MODIFICATIONS**. You can of course modify and add any blocks you wish to your Reaktor rack. For example, you could want to add a quantizer, a clock divider or some utility blocks. The only constraint is to keep the essential wiring on place of the original preset. 

---

