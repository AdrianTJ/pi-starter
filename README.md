# pi profile: pi-starter

A shareable config profile for the [pi coding agent](https://pi.dev), installed with the
pi-profile wrapper: https://github.com/YOUR_USER/pi-profiles

## Install

```sh
pi-profile install YOUR_USER/THIS_REPO   # after pushing this folder to GitHub
```

Packages declared in settings.json are re-fetched from npm/git on first launch —
nothing here is vendored.

## Notes

- Credentials (auth.json, models-store.json) are deliberately not included;
  they are symlinked from your global config at install time.
- Extension entries in settings.json pointing at absolute local paths won't
  resolve on other machines. Publish those extensions as npm/git packages.
- Trust model: installing a profile runs its declared packages, same as any
  npm install. Read settings.json before installing someone else's profile.
