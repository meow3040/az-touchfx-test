# Touch FX for XDJ-AZ

## AZ-MODS repository status

The build workflow publishes **Touch FX (Custom Core)** as a beta panel package
after its regression tests and SDK validation pass. Its Browse entry is added
only after the public release downloads pass the SDK's size, hash and package
checks. Add `meow3040/az-touchfx-test` in AZ-MODS and refresh Browse.

**The package requires matching custom `azmod.so` and `azstem.so` libraries. It
does not run on the standard AZ-MODS core or install those libraries.** Touch FX
0.8.0 needs all three matching components on firmware `ep147-9e9454e357389ece`.
See [PACKAGE-RELEASE.md](PACKAGE-RELEASE.md), [BUILD.md](BUILD.md),
[INSTALL.md](INSTALL.md), and [RESTORE.md](RESTORE.md).

GitHub Actions passed all five existing panel test programs and SDK package
validation. A separate fresh build reproduced all three library hashes in the
original author's [VERIFICATION.json](VERIFICATION.json). This mirror has not
tested the package on hardware. Core/audio binaries and extracted firmware
resources are not distributed here.

## Features

Touch-controlled STEMS and Drum Roll effects with automatic mixer following,
separate panel memory for each deck and adaptive 2, 2/4 and 4-deck layouts.

- STEMS: ECHO, LFO, LFO ECHO, GATE, ROLL and ECHO ROLL.
- STEMS beat choices:4,2,1,3/4,1/2,1/4,1/8,1/16, following live BPM.
- Sampler effects, optional bank1-4 shortcuts and LATCH.
- Colour, no-colour and transparent layouts.
- STEMS colour dimming follows EQ and pad mute states.
- Optional touch control of Kyle's native STEMS buttons.
- Customisable pointer colour, trail and launcher size.
- Native information-column button remains usable through either panel.

## Requirements

**STEMS Touch FX works only with tracks whose stems have been prepared using
Kyle's AZ-MODS Mod Manager, with STEMS enabled on the selected deck.**
Drum Roll/Sampler uses its own samples.

**This version requires the matching customised azmod.so AND azstem.so. Installing
the .azmod package alone on the official core is not sufficient.**
Tested on the author's XDJ-AZ with firmware tag ep147-9e9454e357389ece.
Other firmware/core versions have not been validated. This is an independent
custom build, not an official AZ-MODS release.

## Status

Version 0.8.0 was tested on the original author's player. All three binaries
reproduce from the cleaned source with the pinned toolchain (see
VERIFICATION.json). This mirror publishes the panel as a beta package for
players that already have the matching custom core and audio libraries.
Those libraries are not distributed here. See INSTALL.md, RESTORE.md and
BUILD.md before installation.

## Feedback

Include firmware/AZ-MODS versions, selected deck/view, effect and beat setting,
LATCH state and steps to reproduce. A short video is useful for visual issues.

## Credits and licence

Touch FX by mrdjjag, built on Kyle Hosman's AZ-MODS and SDK.
GPL-3.0-only; upstream and third-party notices are retained in NOTICE and source.
Not affiliated with AlphaTheta or Pioneer DJ.

