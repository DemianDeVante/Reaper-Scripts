# RPC Control and Scripts for Reaper DAW
This is a collection of scripts and custom actions made in order to make MIDI controllers more useful with Reaper.  

## Features
* **RPC Control:**  
  A minimalistic ReaLearn Template in order to achieve a nearly mouseless workflow, influenced by MPC workstations.  
* **Looper D:**  
  A script collection aimed to make live looping easier, taking advantage of the native takes system.
* **Demian D Scripts:**  
  Various scripts made mainly for use with MIDI controllers.
  
## Requirements
### Demian D Scripts & Looper D
* [SWS Extension](https://www.sws-extension.org/)
* [Reapack](https://reapack.com/)
* [ReaScript API](https://forum.cockos.com/showthread.php?t=212174) (available through Reapack).

### RPC Control
* A MIDI controller with at least 17 Pads/Buttons/Triggers and 8 Knobs (all relative/endless) (recommended).
* [ReaLearn](https://www.helgoboss.org/projects/realearn/)
* Demian D Scripts & Looper D
* [Quick Adder](https://forum.cockos.com/showthread.php?t=232928)
* [X-Raym_Move selected tracks up/down on visible track list](https://forum.cockos.com/showthread.php?t=178071) (available through Reapack)

## Installation
To open the Reaper Resource Path go to (Options >> Show Reaper resource path in explorer/finder...).  

![Reaper Resource Path](https://user-images.githubusercontent.com/113860974/191146302-e6bc7f96-15f2-4317-b8bf-177025e5368c.jpg)

### Demian D Scripts & Looper D
* Copy the Scripts folder into Reaper Resource Path.
* Import "Demian D Script Pack.ReaperKeyMap" through: (Action List >> Key map... >> Import shortcut keymap).  

![Import Keymap](https://user-images.githubusercontent.com/113860974/191146345-0d6454f5-3a74-41f0-927d-9cdbc70c0bfb.jpg)

* In (Preferences >> Audio >> Loop Recording)  make sure "At each loop (creates new files, good for recording multiple audio layers on the fly etc)" is disabled.

![Looper D preferences](https://user-images.githubusercontent.com/113860974/191147958-3a531ecc-dfa0-415e-a4f6-1834cdb37cb2.jpg)

### RPC Control
* Copy the Data folder into Reaper Resource Path.
* Go to (Extensions >> Startup actions >> Set global startup action...) and paste the ID of the script "Dem Startup Action.lua" (This script just makes sure Reaper Starts in Fullscreen and Loads Screenset 1. The ID is: _RS6c80eaa8a9a5bdeb85699d81fd67fba0f32f6948).  
* Copy the [sset0] configuration inside "reaper-screensets.ini", alternatively if you don't mind losing your screensets copy the whole file to Reaper Resource Path.
* Import "RPC Control Toolbars.ReaperMenuSet" through: (Options >> Customize menus/toolbars... >> Import/Export >> Import).

![Import Toolbars](https://user-images.githubusercontent.com/113860974/191152689-1eebc6ba-a137-46e6-b8e5-56185eadf565.jpg)

* Open the Monitoring FX (View >> Monitoring FX) and insert a ReaLearn Instance.
* Choose "RPC Control" as controller preset both in main and controller compartment.

![ReaLearn Preset](https://user-images.githubusercontent.com/113860974/191152761-4925c86a-cacb-49d6-941d-784ca8f2858b.jpg)

* In (Controller compartment >> Mapping group >> Knobs/Pads Control Change) assign your MIDI controller knobs and buttons by clicking on "Learn Source".

![ReaLearn Assign Pads Knobs](https://user-images.githubusercontent.com/113860974/191152778-e661e1f2-5b9b-407e-8acb-f5b0068a5d68.jpg)

* In (Controller compartment >> Mapping group >> Modifier) assign the button you want to use as a modifier for changing Modes, alternatively you can assign Program Change messages to do this function.






