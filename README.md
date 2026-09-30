# DataForte AB — brand assets

Public home for the artwork our Forge apps and Marketplace listings point at.

## Why this repo exists

A Forge module's `icon:` field needs a **publicly reachable URL**. Until now our
apps shipped the icon that `forge create` scaffolds —
`https://developer.atlassian.com/platform/forge/images/icons/issue-panel-icon.svg`
— which is Atlassian's own artwork. A Marketplace reviewer flagged it, correctly.

Hosting the icons here keeps them in one place instead of scattering them across
each app's legal-pages repo, and it works for every app regardless of who has
write access to which repository.

## Contents

`icons/<app>.png` — 144×144, the same mark each app uses on its Marketplace
listing, so the listing, the issue panel and the context module agree.

Served at:

```
https://dataforteab.github.io/brand/icons/<app>.png
```

## Adding an app

1. Drop `icons/<app>.png` here (144×144 PNG, transparent corners).
2. Point the app's manifest at the URL above.
3. Check it at 48px before shipping — thin monoline marks disappear at that size,
   which is why the Signature set was chosen over the alternative in August.
