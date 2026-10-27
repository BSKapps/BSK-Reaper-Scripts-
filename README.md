REAPER scripts for virtual soundcheck and live multitrack recording. Mac tested, untested on Windows.

Install with ReaPack: Extensions > ReaPack > Import a repository, paste `https://raw.githubusercontent.com/BSKapps/BSK-Reaper-Scripts-/main/index.xml`, then Browse packages. Or download a script, then in the Actions list use New action > Load ReaScript.

The full live recording setup (toolbars, lights, SAFE REC, REC TIME LEFT, templates and theme) is a free download at https://bskapps.com/tools/reaper/

## AutoPatch

- **AutoPatch HW 1-to-1 Mono and Stereo**: patches every track 1:1 to hardware inputs and outputs. Set a track's input to stereo first and it takes the next pair; the tracks after it move along. Tracks past what your interface has come out blank (no input or output), so nothing doubles up, and a stereo one comes back stereo on a bigger interface.
- **AutoPatch HW 1-to-1 Mono**: the same, every track mono.
- **AutoRoute HW Pre FX**: for every track with a hardware output: outputs pre FX and pre fader, record monitoring off, master send off. Run it after AutoPatch for virtual soundcheck.
- **AutoPatch HW Teardown**: asks first, then removes every track's hardware inputs and outputs and turns master send and record monitoring back on.
- **Reset Volume, Pan and Outputs**: asks first, then faders to 0 dB, pan to centre, every hardware output to 0 dB and centre, every item and take to 0 dB. Needs the SWS extension.

## Track names and colours

- **Import Track Names**: names your tracks from a CSV or text file: sectioned console exports (dLive, Avantis, SQ), standard CSV (Yamaha CL, QL, Rivage) or one name per line. Shows the names before it changes anything.
- **Auto-name Tracks from Device Inputs**: names each track from the input label your interface reports. Shows the names first.
- **Auto Color**: colours (and optionally icons) tracks by words in their names. Edit the groups to suit your desk.

## Transport (for Stream Deck)

- **Safe Rec Play**: starts playback only if stopped or paused, never while recording.
- **Safe Rec Pause**: pauses if playing and unpauses if paused (including a paused recording). Never pauses an active recording.
- **Safe Rec Record**: starts recording only if not already recording, then unselects every track so a fader or mute you touch mid-show moves only that track.
