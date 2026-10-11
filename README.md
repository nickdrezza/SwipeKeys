# SwipeKeys

A tiny macOS app that maps keyboard controls to mouse gestures.

I made this to play Subway Surfers City on my MacBook after enjoying the game a
bit too much.

Made by [Guilherme Drezza](https://nickdrezza.com).

## Portfolio Notes

- **Problem:** some macOS games expect touch gestures even when the useful input device is a keyboard.
- **Approach:** map keyboard shortcuts to cursor-centered swipe and tap gestures while keeping the app tiny, native, and easy to toggle.
- **What it shows:** Swift, macOS input permissions, event monitoring, small native utility design, and release packaging.

## Controls

| Key | Action |
| --- | --- |
| Arrow keys | Swipe |
| Enter | Tap |
| `Command` + `Control` + `Option` + `K` | Toggle on/off |

Actions happen around the cursor. Original key presses still pass through.

Use `Edit` to switch to `WASD` + Space or set custom bindings. Use
`Permissions` to check Accessibility and Input Monitoring.

## Install

Download `SwipeKeys-macOS.zip` from the latest GitHub release, unzip it, and
drag `SwipeKeys.app` into Applications.

SwipeKeys needs:

- Accessibility
- Input Monitoring

Open SwipeKeys, click `Permissions`, enable both in System Settings, then reopen
the app if macOS asks.

## Build

```sh
git clone https://github.com/guidrezza/SwipeKeys.git
cd SwipeKeys
./Scripts/build-app.sh
```

The app is created at `dist/SwipeKeys.app`.

## License

This project is licensed under [GNU AGPLv3 only](LICENSE) (`AGPL-3.0-only`).
See [NOTICE](NOTICE) for copyright information.

You can use, change, and sell copies under the license terms.
If you distribute covered code, provide its source under the same license.
If you change the project and let users access it over a network,
offer those users the source of your version.

Earlier releases keep the license terms that applied to them.
