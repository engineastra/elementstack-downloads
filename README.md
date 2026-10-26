# ElementStack desktop installers

This repository holds the **desktop app installers** for [ElementStack](https://elementstack.vercel.app), a front-end
interview practice app that runs on your own computer. It contains only installers, one release per version. The source
code is not here.

**Get the app from the [ElementStack website](https://elementstack.vercel.app)**, which links to the right file for your
computer. You can also pick a version under [Releases](../../releases).

| File                                   | For                                   |
| -------------------------------------- | ------------------------------------- |
| `ElementStack-<version>-mac-arm64.dmg` | Macs with Apple silicon (M1 or newer) |
| `ElementStack-<version>-mac-x64.dmg`   | Intel Macs                            |
| `ElementStack-Setup-<version>.exe`     | Windows 10 and 11, 64-bit             |
| `<installer>.sha256`                   | The SHA-256 of each installer         |

## Before you run an installer

- **They are not signed yet**, so your computer may warn you the first time. On a Mac, right-click the app and choose Open.
  On Windows, choose More info, then Run anyway.
- **You need Docker** (or a compatible engine such as Docker Desktop, Rancher Desktop, OrbStack or Colima). The app can
  help you install and start it.
- To check a download, compare its SHA-256 with the matching `.sha256` file. On a Mac or Linux, put both files in one
  folder and run `shasum -a 256 -c <installer>.sha256`.

The installers are built and published automatically by the ElementStack release process. Please do not edit this
repository by hand.
