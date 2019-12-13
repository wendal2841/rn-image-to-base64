
# rn-image-to-base64

This repo is a working rewrite of [this](https://github.com/wendal2841/rn-image-to-base64) abandoned library.
It provides a very simple way to convert an image to a base64 string.

If you encounter `OOM` errors on old android devices, make sure you optimize the image's size before you convert it. 
Indeed working with big images on Android might cause very high memory usage.

## Getting started

`npm install rn-image-to-base64 --save`
or
`yarn add rn-image-to-base64`


## Installation

`$ react-native link rn-image-to-base64`

## Usage
```javascript
import ImgToBase64 from 'rn-image-to-base64';

ImgToBase64.getBase64String('file://youfileurl')
  .then(base64String => doSomethingWith(base64String))
  .catch(err => doSomethingWith(err));
```
  
