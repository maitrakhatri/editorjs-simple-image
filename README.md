# Simple Image Tool (without Caption)

Provides Image Blocks (without Caption) for the [Editor.js](https://editorjs.io).

Works for Image drag n drop, pasting images from clipboard and requires no server-side uploader.

## Installation

### Install via NPM

Get the package

```shell
npm i @maitrakhatri/editorjs-simple-image
```

Include module at your application

```javascript
const SimpleImage = require('@maitrakhatri/editorjs-simple-image');
```

OR

```javascript
import SimpleImage from "@maitrakhatri/editorjs-simple-image";
```

### Download to your project's source dir

1. Upload folder `dist` from repository
2. Add `dist/bundle.js` file to your page.

## Usage

Add a new Tool to the `tools` property of the Editor.js initial config.

```javascript
var editor = EditorJS({
  ...
  
  tools: {
    ...
    image: SimpleImage,
  }
  
  ...
});
```

## Config Params

This Tool has no config params

## Tool's settings

![](https://capella.pics/c74cdeec-3405-48ac-a960-f784188cf9b4.jpg)

1. Add border

2. Stretch to full-width

3. Add background

## Output data

| Field          | Type      | Description                     |
| -------------- | --------- | ------------------------------- |
| url            | `string`  | image's url                     |
| withBorder     | `boolean` | add border to image             |
| withBackground | `boolean` | need to add background          |
| stretched      | `boolean` | stretch image to screen's width |


```json
{
    "type" : "image",
    "data" : {
        "url" : "https://www.tesla.com/tesla_theme/assets/img/_vehicle_redesign/roadster_and_semi/roadster/hero.jpg",
        "withBorder" : false,
        "withBackground" : false,
        "stretched" : true
    }
}
```
