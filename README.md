# iMobileDeviceGUI
Windows GUI for [libimobiledevice](https://github.com/libimobiledevice)

![iMobileDeviceGUI Preview](https://github.com/htmiel/iMobileDeviceGUI/blob/master/preview.png)

This is a small Windows tool for installing, removing or updating apps on iOS devices.

## Usage

- Add .ipa files using the `+` button on the lower left side. Added apps will be visible on the left side.
  - By default, your apps will show the default icon. To add a custom icon for each app, add a 64x64 png file in the `appIcons` folder of the application, and name it in the following format: `bundle_id.png` (ex: `com.funnygames.flappydragon.png`)
- Plug in your iOS device. It will appear on the right side.
- Select an app from the list on the left side. It will turn blue.
  - If your device does not have a preview or you don't like the default one, you can change that in the `deviceIcons` folder of the application. Preview files are named after device IDs (https://gist.github.com/adamawolf/3048717). Device previews should have 82 pixels height (80 + 1 pixel white outside stroke on all sides)
- For each device you want, press `Install`, `Remove` or `Update`
- Remove apps from the list by pressing the `-` button on the lower left side.

**Extras:**
- Each app updates the following information: .ipa file size, version and time since it was compiled.
- For each device, you can press the `Copy` button to copy to clipboard: device name and model ID, iOS version and device unique ID.
