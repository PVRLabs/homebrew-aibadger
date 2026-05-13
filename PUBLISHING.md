# Publishing Guide

This tap is the public Homebrew entry point for `badger`.

## Initial Publish

1. Create the GitHub repository `PVRLabs/homebrew-aibadger`.
2. Push this directory to that repository.
3. Confirm the default branch contains:
   - `Formula/badger.rb`
   - `README.md`
   - `PUBLISHING.md`
4. Make sure the repo is public.

## After Each `aibadger` Release

1. Update `Formula/badger.rb` with the new `version` and SHA-256 values.
2. Keep the formula URLs pointed at the GitHub Release assets for
   `github.com/PVRLabs/aibadger`.
3. Verify the archive names still match the release workflow.
4. Confirm the version output remains `badger v<version>`.

## Validation

Use a clean machine or clean Homebrew environment to verify:

```bash
brew tap pvrlabs/aibadger
brew install pvrlabs/aibadger/badger
badger --version
```

## Notes

- Keep this tap minimal.
- Do not add private sidecar docs here.
- Only publish metadata needed for installation and maintenance.
