# ProLink Bridge 4.0 Beta

**Behringer WING · Behringer X32 / Midas M32 → Waves SuperRack SoundGrid (ProLink)**

Press **SELECT** on the console and the SuperRack rack on the **same card channel** opens — in real time, as the console is routed right now.
**Touch and Turn** from the assignable encoders of the full-size consoles, or from any MIDI controller with endless knobs.

---

## Download

| Console | Mac — Apple Silicon (M1–M4) | Mac — Intel | Windows 10 / 11 |
|---|---|---|---|
| **Behringer WING** | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-WING-4.0-Beta-Mac-Apple-Silicon.dmg) | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-WING-4.0-Beta-Mac-Intel.dmg) | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-WING-4.0-Beta-Windows.zip) |
| **Behringer X32 / Midas M32** | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-X-M32-4.0-Beta-Mac-Apple-Silicon.dmg) | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-X-M32-4.0-Beta-Mac-Intel.dmg) | [Download](https://github.com/victorastulum065/VictorBridge-beta-v4/releases/download/v4.0-beta/ProLink-Bridge-X-M32-4.0-Beta-Windows.zip) |

Which Mac? Apple menu › About This Mac › **Chip** (Apple M…) or **Processor** (Intel).

## Works with (tested)

| | Version |
|---|---|
| Waves SuperRack SoundGrid | **15.15** (ProLink) |
| Behringer WING / WING Rack / WING Compact | firmware **3.1** |
| Behringer X32 / Midas M32 (all models, M32R included) | firmware **4.13** |
| Mac | macOS **10.15** or newer — Apple Silicon or Intel |
| Windows | Windows **10 / 11**, 64-bit — nothing else to install |

---

## Install

**Mac**
1. Open the `.dmg`, drag the app onto **Applications**, open it.
2. If macOS says it cannot check the app: **System Settings › Privacy & Security › Open Anyway** (older macOS: right-click › Open › Open).
3. Allow it to find devices on the local network. The panel opens in your browser.

**Windows**
1. Unzip the `.zip` (right-click › Extract All).
2. Right-click **Allow through the firewall.cmd** › **Run as administrator** (once).
3. Start the `.exe`. If you see *"Windows protected your PC"*: **More info › Run anyway**.

## How to connect — 3 steps

1. **Network** — console and the SuperRack computer on the same network, same IP range (e.g. `192.168.0.x`).
2. **Bridge** — in the panel press **Start**. The console is found by itself; if not, *Type the console address* (console: Setup › Network).
3. **SuperRack** — **Setup › ProLink › "ProLink Console Remote"**, then pick the console in the list. The SuperRack light in the panel turns green.

Run only one bridge per computer.

---

## SELECT — all consoles, all models

- Opens the rack that sits on the **same card channel** in SuperRack (channel 5 from card 45 → the rack on card 45).
- Stereo channels open one rack. Buses, main and matrices follow their insert or card output.
- **WING:** follows the **ALT** source when it is on, and external FX inserts returning on the card.
- **A source with no matching card channel opens nothing.**
- Real time: change a source, the routing, an insert, a scene or a rack — it updates in under a second. Names are never used.

## Touch and Turn — full-size consoles only

Works on **Behringer WING, Behringer X32 and Midas M32**, from their assignable encoders, or from an external MIDI controller with endless knobs.

| Console / device | What to do |
|---|---|
| **WING** | Custom Controls (USER / LAYER): set the knob to **MIDI CC**. In the panel tick *Touch and Turn on every Custom Control encoder*, or bind one knob with *Listen*. |
| **X32 / M32** | Setup › **User Assign**: give the Assign encoder a function. Bank C encoder 1 is Touch and Turn out of the box. |
| **MIDI controller** | *Setup › External MIDI controller* › pick it › **Listen** › turn a knob › **Pick** › *Touch and Turn — relative MIDI encoder* › **Bind**. |

Any other function (open a rack, next / previous plugin, snapshots, tap tempo…) goes on any button the same way.

## MIDI functions

1. **Console → SuperRack over the network cable.** The bridge appears as a MIDI port: buttons send notes, encoders send endless CCs. In SuperRack: Setup › MIDI, pick the port, right-click a parameter › MIDI Learn.
2. **Choose what each control sends** — *Setup › What each console control sends*: note or CC, MIDI channel, number, on / off / auto, and a **Send** button for MIDI Learn.
3. **MIDI controller → bridge** — any MIDI box or keyboard on the computer can drive bridge functions.
4. **Windows:** the port to SuperRack needs **loopMIDI** (free) — create one port and pick it in Setup.

## Gain — X32 / M32

- The GAIN knob moves the **real preamp** of the channel (local, AES50 A or B), read from the console **in real time**; the digital trim stays at 0 dB.
- *Extra › Gain routing*: send any channel's gain wherever you want; **Auto** gives it back to the routing.
- *Extra › Gain box*: show, move and size the small on-screen gain box.

## Scenes — Extra, off by default

- *Every scene remembers its bridge setup*: save in SuperRack or on the console and your SELECT pins and controls are kept with that console scene, and come back with it.
- What you change stays as you left it, also after you reopen the program.
- X32 / M32: SAVE / RECALL on the console can also save / open the SuperRack session.

## The panel

| Tab | What is there |
|---|---|
| **Main** | Start / Stop, Console / SuperRack / Scene lights, licence (X32/M32: GAIN on TRIM) |
| **Setup** | SELECT by card, Touch and Turn & controls, MIDI |
| **Extra** | Gain routing and gain box (X32/M32), scenes and sessions, rack names, log |

## Demo and licence

- The demo runs **30 minutes** each time you open it, then disconnects — quit and open it again for another 30 minutes.
- **Licence:** copy the code shown under *Licence* in the panel and send it on **Facebook Messenger** or to **victorastulum065@gmail.com**. Paste the key you receive and press **Activate**.
- One licence = one computer. Works offline.

---

© Tulum Victoraș Mirel. All rights reserved. This repository contains only the program packages; no part of it may be redistributed, modified or reverse-engineered.
WING, X32 and M32 are trademarks of their owners. SuperRack and SoundGrid are trademarks of Waves Audio. ProLink Bridge is an independent product.
