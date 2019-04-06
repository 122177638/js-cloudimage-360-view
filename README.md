[![Release](https://img.shields.io/badge/release-v0.0.3-blue.svg)](https://github.com/scaleflex/js-cloudimage-360-view/releases)
[![Contributions welcome](https://img.shields.io/badge/contributions-welcome-orange.svg)](#contributing)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Scaleflex team](https://img.shields.io/badge/%3C%2F%3E%20with%20%E2%99%A5%20by-the%20Scaleflex%20team-6986fa.svg)](https://www.scaleflex.it/en/home)

[![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=Engage%20your%20customers%20with%20a%20stunning%20360%20viewvof%20your%20products&url=https://scaleflex.github.io/js-cloudimage-360-view/&via=cloudimage&hashtags=images,cloudimage)

<p align="center">
	<img
		height="175"
		alt="The Lounge"
		src="https://demo.cloudimg.io/height/350/n/https://scaleflex.airstore.io/filerobot/filerobot-cloudimage.png?sanitize=true">
</p>

<h1 align="center">
   JS Cloudimage 360 View
</h1>

<p align="center">
	<strong>
		<a href="#table_of_contents">Docs</a>
		•
		<a href="https://scaleflex.github.io/js-cloudimage-360-view/" target="_blank">Demo</a>
		•
		<a href="https://codesandbox.io/s/6479n17j73?fontsize=14&module=%2Findex.html" target="_blank">Code Sandbox</a>
	</strong>
</p>

A simple, interactive resource that can be used to provide a virtual tour of your product.

<p align="center">
	<img
		alt="The Lounge"
		src="https://scaleflex.ultrafast.io/https://scaleflex.airstore.io/filerobot/js-cloudimage-360-view/demo-360-small.gif?sanitize=true">
</p>

powered by [Cloudimage](https://www.cloudimage.io/)
([Watch the video here](https://www.youtube.com/watch?time_continue=2&v=JFZSE1vYb0k))

## Table of contents

* [Demo](#demo)
* [Step 1: Installation](#installation)
* [Step 2: Initialize](#initialize)
* [Configuration](#configuration)
* [Best practices](#best-practices)
* [Browser support](#browser_support)
* [Filerobot UI Family](#ui_family)
* [Contributing](#contributing)
* [License](#license)


## <a name="demo"></a> Demo

To see the Cloudimage 360 view plugin in action, please check out the
[Demo page](https://scaleflex.github.io/js-cloudimage-360-view/).

## <a name="installation"></a>Step 1: Installation

Add script tag with CDN link to js-cloudimage-360-view lib after all content in body tag

```javascript
<script src="https://cdn.scaleflex.it/filerobot/js-cloudimage-360-view/v0.0.3.min.js"></script>
```

or using npm

```
$ npm install --save js-cloudimage-360-view
```

```javascript
import 'js-cloudimage-360-view';
```

## <a name="initialize"></a>Step 2: Initialize

After adding the js-cloudimage-360-view lib, simply iniatialize it with **class name "cloudimage-360"**,
**server folder path**, **file name** and amount of images:

```html
<div
   class="cloudimage-360"
   data-folder="https://scaleflex.cloudimg.io/crop/1920x700/n/https://scaleflex.airstore.io/demo/360-car/"
   data-filename="iris-{index}.jpeg"
   data-amount="36"
></div>
```

<a href="https://codesandbox.io/s/6479n17j73?fontsize=14&module=%2Findex.html"><img src="https://codesandbox.io/static/img/play-codesandbox.svg" alt="edeit in codesandbox"/></a>

## <a name="configuration"></a> Config

### class

###### Type: **String** | Value: **"cloudimage-360"** | _required_

The selector for js-cloudimage-360-view lib.

### data-folder (or folder)

###### Type: **String(url)** | _required_

Your images folder on server.

### data-amount (or amount)

###### Type: **Number** | Default: **36** | _optional_

Amount of images to load for 360 view.

### data-keys (or keys)

###### Type: **Bool** | Default: **false** | _optional_

Support for 360 spin by pressing arrow keys on keyboard.

### data-autoplay (or autoplay)

###### Type: **Bool** | Default: **false** | _optional_

Autoplay 360 spin view on load.

### data-full-screen (or full-screen)

###### Type: **Bool** | Default: **false** | _optional_

Open 360 spin view in full screen modal.

### data-magnifier (or magnifier)

###### Type: **Number** | Default: **none** | _optional_

Magnifier to zoom image.

### data-ratio (or ratio)

###### Type: **Number** (height / width) | Default: **none** | _optional_

Prevents page from jumping.

### data-autoplay-reverse (or autoplay-reverse)

###### Type: **Bool** | Default: **false** | _optional_

Autoplay 360 spin view on load.

### data-speed (or speed)

###### Type: **Number** | Default: **150** | _optional_

Speed of changing frames in milliseconds.

### data-box-shadow (or box-shadow)

###### Type: **String** (e.g. data-box-shadow="inset 0 0 100px #222") | Default: **none** | _optional_

Apply box shadow for container.

### data-bottom-circle (or bottom-circle)

###### Type: **Bool** | Default: **false** | _optional_

Display 360 view line at the bottom of container.

### data-bottom-circle-offset (or bottom-circle-offset)

###### Type: **Number** | Default: **5** | _optional_

Bottom offset for 360 view line.

## <a name="best-practices"/> Best practices

* In order to use cloudimage responsive with 360 view, your original (master) images should be stored on a server
or storage bucket (S3, Google Cloud, Azure Blob...) reachable over
HTTP or HTTPS by Cloudimage. If you want to upload your master images to
Cloudimage, contact us at
[hello@cloudimage.io](mailto:hello@cloudimage.io).

## <a name="browser_support"></a> Browser support

Tested in all modern browsers and IE 11, 10, 9.

## <a name="ui_family"></a>Filerobot UI Familiy

* [JS Cloudimage Responsive](https://github.com/scaleflex/js-cloudimage-responsive)
* [React Cloudimage Responsive](https://github.com/scaleflex/react-cloudimage-responsive)
* [Angular Cloudimage Responsive](https://github.com/scaleflex/ng-cloudimage-responsive)
* [Image Editor](https://github.com/scaleflex/filerobot-image-editor)
* [Uploader](https://github.com/scaleflex/filerobot-uploader)

## <a name="contributing"></a>Contributing!

All contributions are super welcome!

## <a name="license"></a>License
JS Cloudimage 360 View is provided under the [MIT License](https://opensource.org/licenses/MIT)

