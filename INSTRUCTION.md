# Setup project

## Clone source code

```bash
git clone https://github.com/toanalien/react-native-starter-kit-instamobile.git
```

## Install Node modules

```bash
yarn install
```

## Install dependency for iOS

```bash
pod install
```

## Install third party for React Native

```bash
cd node_modules/react-native/third-party/glog-0.3.4/ && ../../scripts/ios-configure-glog.sh && cd ../../../../
```

## Run app on iOS device

```bash
react-native run-ios
```

# Fix Issue

- Build input file cannot be found: `'node_modules/react-native/Libraries/WebSocket/libfishhook.a'`

![](https://i.imgur.com/bXznJf3.png)

- Remove & re-add `libfishhook.a` in Xcode

![](https://i.imgur.com/FT8PkYS.png)

![](https://i.imgur.com/7GUmobE.png)

![](https://i.imgur.com/4xBQIFQ.png)

- Re-build Project

![](https://i.imgur.com/sxrnRoF.png)