# homebrew-tap

My custom tap of Homebrew formulas. At the moment there is a single one
here – OpenSSH with a patch to support ECDSA keys from smartcards.
The patch is from [OpenSSH Bugzilla](https://bugzilla.mindrot.org/show_bug.cgi?id=2474)
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

## Notes

With patch applied OpenSSH outputs 'C_GetAttributeValue failed: 18' warnings
when smartcard is accessed. These warnings are harmless.
