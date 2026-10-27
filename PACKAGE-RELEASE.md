# Touch FX 0.8.0 - custom core required

This beta release contains the Touch FX **panel package only**. It requires the
matching customised `azmod.so` and `azstem.so` from the original Touch FX 0.8.0
bundle, on firmware `ep147-9e9454e357389ece`. It does not run on the standard
AZ-MODS core and does not replace or install those two libraries.

With those prerequisites already installed, add `meow3040/az-touchfx-test` in
AZ-MODS, refresh Browse and select **Touch FX (Custom Core)**. Follow
[INSTALL.md](https://github.com/meow3040/az-touchfx-test/blob/main/INSTALL.md).
For building the required core and audio libraries yourself, see
[BUILD.md](https://github.com/meow3040/az-touchfx-test/blob/main/BUILD.md).

The package was built with the SDK commit recorded in `PROVENANCE.json`.
All five existing panel test programs and the SDK's library/package validation
passed in GitHub Actions. A separate fresh build reproduced all three original
library hashes from `VERIFICATION.json`. This establishes build reproduction,
not a hardware test performed by this repository's maintainer.

STEMS tracks must be prepared with Kyle's AZ-MODS Mod Manager and enabled on
the selected deck. Sampler/Drum Roll uses its own samples.

Touch FX is by mrdjjag, based on Kyle Hosman's AZ-MODS and SDK. This repository
provides a build mirror. Original authorship, module ID and GPL-3.0-only licensing
are retained. No custom core binary, firmware arrays or database key bytes are
attached to this release.
