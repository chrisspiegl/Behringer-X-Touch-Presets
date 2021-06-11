# [Behringer X-Touch Mini](https://crsp.li/xtouchmini) Button Layer A/B Presets

These files can be loaded with the [Behringer X-Touch Editor](https://www.behringer.com/product.html?modelCode=P0B3M). Sadly this editor is only available on Windows and not for macOS and the only known workaround is to use a virtual machine via [VirtualBox](https://www.virtualbox.org/).

## Purpose

By default the [X-Touch Mini](https://crsp.li/xtouchmini) is not setup very "logical" with it's notes, dials, and faders. The notes and buttons are are rather random in their numbering.

With these presets the numbering is much more logical and easy to remember.

## Installation

[Full Video Tutorial / Walkthrough](https://youtu.be/nOtiOq8SkG8)

[![Video Tutorial on YouTube](http://i3.ytimg.com/vi/nOtiOq8SkG8/maxresdefault.jpg)](https://youtu.be/nOtiOq8SkG8)

1. Download this Repository ([ZIP](https://github.com/chrisspiegl/Behringer-X-Touch-Presets/archive/refs/heads/main.zip))
2. Extract the ZIP Archive
3. Download the [Behringer X-Touch Editor](https://www.behringer.com/product.html?modelCode=P0B3M)
4. Launch Windows in a Virtual Machine (if you are on Linux or macOS)
	- You can download a Windows for testing purposes from [Microsoft directly](https://developer.microsoft.com/en-us/windows/downloads/virtual-machines/).
5. Load Layer A file (`Behringer-X-Touch-Mini-Layer-A-v1.bin`) into Behringer X-Touch Editor
6. Click on `Dump A` and confirm
7. Load Layer B file (`Behringer-X-Touch-Mini-Layer-B-v1.bin`) into Editor
8. Click on `Dump B` and confirm
9. Your MIDI Controller now has the new button layouts installed. You can check these with a free program called [Protokol](https://hexler.net/protokol) to make sure the right notes are played on the right button press and twist actions.

## Feedback, Bugs, and Issues

Please [create an issue](https://github.com/chrisspiegl/Behringer-X-Touch-Presets/issues/new) on this repository.

## Button & Dial Layout Logic

Twisting the twist dials will send **CONTROL CHANGE** with values from **0** to **127**.

Pressing the twist dials will send **NOTE_ON** with value **127** on press and **NOTE_OFF** with value **0** on release.

All buttons are sending **NOTE_ON** with value **127** on press and **NOTE_OFF** with value **0** on release.

The Fader sends **CONTROL CHANGE** with values between **0** and **127**.

### Notes on Layer A

- Press or twist row of twist dials: 0 - 7
- Press 1st row of buttons: 8 - 15
- Press 2nd row of buttons: 16 - 23
- Fader: 126

### Notes on Layer A

- Press or twist row of twist dials: 24 - 31
- Press 1st row of buttons: 32 - 39
- Press 2nd row of buttons: 40 - 47
- Fader: 127
