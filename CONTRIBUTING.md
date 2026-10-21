# Contributing

Knight Rider style KITT chaser animation for the MacBook Pro Touch Bar (a fork of AkdM/KnightTouchBar2000).

Bug reports and feature requests are welcome as [issues](https://github.com/maubergine/DMWTouchBar/issues). Pull requests are
welcome too; CI on a pull request from a fork may wait for the maintainer to approve it.

## Commits

Use [Conventional Commits](https://www.conventionalcommits.org/): `fix:`, `feat:`, `chore:`, `docs:` and so on. This
fork doesn't cut releases, so the type only describes the change. CI checks every commit (`commitlint.yml`). To check them locally before you push:

```sh
npm install   # installs commitlint and turns on .githooks/commit-msg
```

Commits to `master` must be signed.

## Tests

CI parses the Swift sources with `swiftc -parse -swift-version 4 KnightTouchBar2000/*.swift`. The project no longer builds on current Xcode (Swift 3 settings, pre-rename AppKit APIs).
