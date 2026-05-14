# CrashBytes Homebrew Tap

Homebrew formulas for CrashBytes CLIs.

## Install

```sh
brew install CrashBytes/tap/pipemason
```

(After the first install, `brew upgrade pipemason` keeps it current.)

## What's here

| Formula | What it is |
|---|---|
| `pipemason` | Local runner for the [pipemason](https://pipemason.com) development pipeline. Compiled, code-signed and notarized binary. macOS arm64/x64 and Linux arm64/x64. |

Windows users: Homebrew doesn't ship Windows binaries. Use the `.exe`
attached to each [GitHub Release](https://github.com/CrashBytes/pipemason/releases),
or the one-liner installer documented at [pipemason.com](https://pipemason.com).

## How updates happen

This tap is updated automatically by the `bump-homebrew-tap` job in
[CrashBytes/pipemason](https://github.com/CrashBytes/pipemason)'s release
workflow. Each `v*` tag pushed to that repo triggers a fresh build, signs
and notarizes the macOS targets, publishes a GitHub Release, then pushes
a regenerated `Formula/pipemason.rb` here.

Do not hand-edit `Formula/pipemason.rb` — your changes will be overwritten
on the next release.

## Reporting issues

- **CLI bugs / behavior** → file at [CrashBytes/pipemason](https://github.com/CrashBytes/pipemason/issues).
- **Formula problems** (won't install, wrong SHA, missing platform) → file
  here.
