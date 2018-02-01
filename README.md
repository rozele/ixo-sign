# IXO Sign App

This app is built with [React Native](https://github.com/facebook/react-native).

## Getting Started

### System Requirements

Install the following prerequisites:

- [Node LTS](https://nodejs.org/) (currently 8.9.4)
- NPM v5.5.1
- [Android Studio](https://developer.android.com/studio)

Install the React Native CLI:

```
npm i -g react-native-cli
```

### Running the app

Clone the repository:

```
git clone https://github.com/ixofoundation/ixo-sign
```

In the cloned repo directory, run NPM install:

```
npm i
```

NPM install will generate a `shim.js` file, as well as patch up some Node dependencies from [`ixo-module`](https://github.com/ixofoundation/ixo-module) to work with React Native.

Start an Android emulator or connect a device. Start the app.

```
react-native run-android
```

## Sideload the bundled app

TODO

## Run the app on an alternate packager

It's likely that you'll want to run this app at the same time you're debugging another app (e.g., [IXO Mobile](https://github.com/ixofoundation/ixo-mobile)). In this case you may need to run the packager on a port other than 8081. Here are the instructions:

```
react-native start --port=8082
react-native run-android --no-packager
```

When the app first starts, you're likely to get a red box exception. To resolve this exception, open the dev menu (CMD+M on Mac, Menu key on Windows). Go to the dev settings page and change the configured packager URL to `localhost:8082`.