# homebrew-tap

[![Build Status](https://travis-ci.org/hasso/homebrew-tap.svg?branch=master)](https://travis-ci.org/hasso/homebrew-tap)

My custom tap of Homebrew formulas. At the moment there is a single one
here – OpenSSH with a patch to support ECDSA keys from smartcards.
The patch is written by Mathias Brossard (see [OpenSSH Bugzilla](https://bugzilla.mindrot.org/show_bug.cgi?id=2474) for details)
and the formula is otherwise identical to the one in Homebrew.

## How to install

If you have openssh from Homebrew core installed, you must uninstall it:

```bash
> brew uninstall openssh
```

Then install the one form this repository:

```bash
> brew tap hasso/homebrew-tap
> brew install hasso/homebrew-tap/openssh
```

