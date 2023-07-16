# react-native-card-view-plus [![npm version](https://img.shields.io/npm/v/react-native-cardview-plus.svg?style=flat)](https://www.npmjs.com/package/react-native-cardview-plus) [![npm downloads](https://img.shields.io/npm/dm/react-native-cardview.svg?style=flat-square)](https://www.npmjs.com/package/react-native-cardview-plus) ![Platform - Android and iOS](https://img.shields.io/badge/platform-Android%20%7C%20iOS-yellow.svg) ![MIT](https://img.shields.io/dub/l/vibe-d.svg)

[![npm](https://nodei.co/npm/react-native-cardview-plus.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-native-cardview-plus)

Native CardView that compatible for iOS and Android( both lollipop and pre-lolipop).

##### [Material Design Card Spec](https://www.google.com/design/spec/components/cards.html)

##### [CardView Android Documentation](http://developer.android.com/intl/zh-tw/reference/android/support/v7/widget/CardView.html)

## Features

This is a fork of [react-native-cardview](https://github.com/Kishanjvaghela/react-native-cardview) with the following differences,

- Relax React Native version
- Reduce publish package size
- Add types
- Add web support

## Getting started

```bash
$ npm install react-native-cardview-plus --save
```

## Usage

![N|Example](https://github.com/ratson/react-native-cardview-plus/raw/master/docs/Example-Snapshot.png)

![N|Example](https://github.com/ratson/react-native-cardview-plus/raw/master/docs/ezgif-4-b87dbfaf72.gif)


## Example

Browse the files in the [/example](https://github.com/ratson/react-native-cardview-plus/tree/master/example) directory.

```javascript
import CardView from 'react-native-cardview-plus'
<CardView
          cardElevation={2}
          cardMaxElevation={2}
          cornerRadius={5}>
          <Text>
              Elevation 0
          </Text>
</CardView>
```

## Attributes

- **cardElevation** (Android/iOS)

An attribute to set the elevation of the card. This will increase the 'drop-shadow' of the card.
There can be some performance impact when using a very high elevation value.

- **cardMaxElevation** (Android)

An attribute to support shadow on pre-lollipop device in android. [cardMaxElevation](http://developer.android.com/intl/zh-tw/reference/android/support/v7/widget/CardView.html)

- **cornerRadius** (Android/iOS)
  An attribute to set the radius of the card.

- **useCompatPadding** (Android)

CardView adds additional padding to draw shadows on platforms before Lollipop. [setUseCompatPadding](https://developer.android.com/reference/android/support/v7/widget/CardView.html#setUseCompatPadding(boolean))

- **cornerOverlap** (Android)

On pre-Lollipop platforms, CardView does not clip the bounds of the Card for the rounded corners. Instead, it adds padding to content so that it won't overlap with the rounded corners. You can disable this behavior by setting this field to false.

Setting this value on Lollipop and above does not have any effect unless you have enabled compatibility padding. 

[setPreventCornerOverlap](https://developer.android.com/reference/android/support/v7/widget/CardView.html#setPreventCornerOverlap(boolean))
