# Reason12-AKAI-Midimix-integration
Repository containing necessary files for the integration of Reason 12 and AKAI Midimix controller. This integration is based on original files which were downloaded from Luke Lengl repository https://github.com/lukelengl/AkaiMIDIMixPropellerheadReasonRemote. Enhancements are associated with modified remote codec file __MIDImix.lua__ and mapping file __MIDImix.remotemap__ for Reason 12 and previous versions. I have implemented support for SOLO button. If you press/hold the SOLO button and press a MUTE button coressponding to the one of mixer channels, the rest of channels become inactive/muted and leds shine for them in mute state - the MUTE led for unmuted/solo channel doesn't shine as it shouldn't shine. Next, the SOLO button should be pressed and MUTE button for unmuted/solo channel to unmute all muted channels. I think that this is correct mixer's behavior now. I did two mapping examples for mixers 14:2, 6:2 to demonstrate that everything works correctly. In Reason, you should use 'Lock AKAI Midimix to this device' to work with mixers mentioned above. Also, you can map all faders, knobs, buttons to different devices with the use of 'Edit Remote Override Mapping' option.

## Installation
Copy files __MIDImix.lua, MIDImix.luacodec, MIDImix.png__ to following directory [Reason installation directory]\Remote\DefaultCodecs. In case of Windows OS, the default path should be similar to C:\Program Files\Propellerhead\Reason 12\Remote\DefaultCodecs. Next, copy the file __MIDImix.remotemap__ to the directory [Reason installation directory]\Remote\DefaultMaps\Akai (C:\Program Files\Propellerhead\Reason 12\Remote\DefaultMaps\Akai). Regarding Mac OS, above-mentioned directories should be located in HD/Library/Application Support/Propellerhead Software/Remote.

## Mapping associated with Reason Devices
+ Mixer 14:2
+ Mixer 6:2
+ Combinator (implemented by Luke Lengl)

## Global mappings (implemented by Luke Lengl)
+ Bank Left button will target the previous track in the sequencer.
+ Bank Right button will target the next track in the sequencer.

## License
Please share these files for all people who have Reason and AKAI Midmix so that they could use the good and cheapest DAW mixer (with its full functionality) in Reason DAW.

## Contact
Michał Petaś (majkyxyz@gmail.com)
