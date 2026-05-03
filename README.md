# GamerPad macOS Server Releases

Official release repository for the macOS build of GamerPad.

This repository is used to publish signed `.dmg` installers for the macOS server application. It is intended for end users who want to download the latest release without building the app from source.

## What GamerPad Does

GamerPad turns your macOS machine into a local gamepad host and exposes a virtual controller to the system using Apple's HID and system extension stack. The app is designed so a phone or another device on the same local network can act as the controller input source.

The macOS app is used together with the GamerPad mobile apps:

- Android: https://play.google.com/store/apps/details?id=com.coreorbits.gamerpad
- iPhone: https://apps.apple.com/us/app/gamerpad-phone-gamepad/id6751446324

Install the macOS server on your Mac, then connect from the GamerPad mobile app on the same local network.

## Downloads

Download the latest installer from the [Releases](../../releases) page.

Each release includes:

- `CoreOrbits-GamerPad.dmg`

## Installation

1. Download the latest `.dmg` file from the Releases page.
2. Open the disk image.
3. Drag `CoreOrbits-GamerPad.app` into `Applications`.
4. Launch the app from `Applications`.
5. Install GamerPad on your phone:
   - Android: https://play.google.com/store/apps/details?id=com.coreorbits.gamerpad
   - iPhone: https://apps.apple.com/us/app/gamerpad-phone-gamepad/id6751446324
6. Make sure your Mac and phone are on the same local network.
7. If macOS asks for system extension approval, follow the on-screen steps in System Settings.
8. Open the mobile app and connect to your Mac.

If the connection does not work on the first try, fully quit and restart the GamerPad app on your Mac, then try connecting again from the mobile app.

## System Extension Permission

If you want to manage the extension permission manually:

1. Open `System Settings`.
2. Go to `General`.
3. Open `Login Items & Extensions`.
4. Scroll down to the `Extensions` section.
5. Find the GamerPad app.
6. Click the info button on the right side.
7. Enable the required permission.

You can disable the permission again from the same screen at any time.

You can also disable the extension from inside the app if that option is available in your current version.

## Requirements

- macOS 15.4 or later
- Apple Silicon or Intel Mac supported by the shipped build
- Permission to approve required system extension prompts

## Notes

- Releases in this repository are distributed as notarized macOS binaries.
- Source code, internal build scripts, and development assets are not distributed here.
- If you need the development source repository, use the separate source project maintained by CoreOrbits.

## Support

If installation or launch fails, open an issue in this repository and include:

- macOS version
- device architecture
- the release version you installed
- any visible error message or Gatekeeper/system extension prompt

## License

The binaries and repository contents are distributed under the proprietary license in [LICENSE](../LICENSE.release-repo).
