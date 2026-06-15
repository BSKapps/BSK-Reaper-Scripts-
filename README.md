REAPER scripts to make virtual soundcheck and live multitrack record sessions faster to setup.

In actions menu make new ReaScript, paste this in and hit cmd+s to save. Add the action to a toolbar button or keyboard shortcut for quick access or run from actions menu when needed.

Auto patch sees how many tracks you have and makes each one mono input and mono output to the matching hardware. eg dante DVS standard licence will patch 64 tracks in/out to your DVS.

Just insert multitracks in REAPER and hit autopatch. It will skip any tracks that don't fit to the hardware in/out count and pop up a confirmation message to show what it has done. So track 1/ Input 1/ Output 1. It also sets sends prefade/premute/prefx and disables record monitoring and master sends.

Note on stereo: AutoPatch treats every track as mono and maps track 1 to channel 1, track 2 to channel 2 and so on. If you record a stereo source like overheads or keys, put it on two mono tracks (left and right on their own tracks). A single stereo track only grabs one channel and pushes every track below it out of line.

The teardown script resets all tracks to unassigned inputs and outputs.

The Play/Pause/Rec Transport safe scripts all ignore their main function when recording, so only stop will end a recording. They will function as play/pause/rec normally. For use with Stream Deck buttons
