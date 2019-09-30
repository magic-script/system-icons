# system-icons module
A module that contains the Lumin system icons that can optionally be used with a React Native project that utilizes the [react-native-magic-script](https://github.com/magic-script/react-native-magic-script) library. After installing this module, the magic-script components will automatically use the new icons.

## Install steps
Prerequisites: app should base on React-Native >= 0.60.0
- in main folder of your app create `assets/icons` folder (if it doesn't exist): `mkdir -p assets/icons`
- add `system-icons` to your project dependencies eihter by:
`yarn add git+https://github.com/magic-script/system-icons` or `npm install --save git+https://github.com/magic-script/system-icons`
- execute `yarn` or `npm install`
- create (or update if it exists) `react-native.config.js` with lines:
```
module.exports = {
  assets: ['./assets/icons'],
};
```
- execute `react-native link`
```
$ react-native link
info Linking assets to ios project
warn Group 'Resources' does not exist in your Xcode project. We have created it automatically for you.
info Linking assets to android project
success Assets have been successfully linked to your project
```
All system-icons files are copied into desired location and linked into the platform specific code.