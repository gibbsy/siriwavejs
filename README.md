![image](https://s3.amazonaws.com/f.cl.ly/items/2r2i3p2G262M271N0F2M/siri.gif)

[![Gitter](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/CaffeinaLab/SiriWaveJS?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Have you ever thought on how to get the Siri wave effect on your website or mobile app?

SiriWaveJS is a library that *easily* allows  you to get this effect.

**Embed the script... and Surf!**

#### [LIVE EXAMPLE!](http://kopiro.github.io/siriwavejs)

## Usage

```html
<div id="siri-container"></div>
<script src="/path/to/your/siriwave.js"></script>
<script>
var siriWave = new SiriWave({
	container: document.getElementById('siri-container'),
	width: 640,
	height: 200,
	/*
	speed: 0.2,
	color: '#000',
	frequency: 2
	*/
});
</script>
```

## Constructor options

#### `style` (String, default: 'none')

* `default` - Default iOS9- style
* `ios9` - Style of for iOS9+

#### `container` (DOM Object)

The DOM container where the `canvas` to draw the wave is added.

#### `[speed]` (Number, from `0` to `1`, default: `0.1`)

The speed of the wave.

#### `[amplitude]` (Number, from `0` to `1`, default: `1`)

The noise (amplitude) of the wave.

#### `[frequency]` (Number, from `0` to `N`, default: `1`)

The frequency of the wave.

**Not available in iOS9 Style**

#### `[color]` (String, Color, default: `#fff`)

The color of the wave, in hexadecimal form (`#336699`, `#FF0`)

**Not available in iOS9 Style**

#### `[cover]` (Boolean, default: `false`)

The `canvas` covers the entire width or height of the container.

#### `[speedInterpolationSpeed]` (Number)

The speed to interpolate the `speed` property.

#### `[amplitudeInterpolationSpeed]` (Number)

The speed to interpolate the `amplitude` property.

#### `[fps]` (Number)

Enter a number to throttle requestAnimationFrame using setTimeout. Enter 60 for no throttling.

#### `[smoothness]` (Number, from `1` to `10`, default: `1`)

1 for less smooth curve but better performance. 10 = max smoothness;

## API

#### `start()`
Start the animation

#### `stop()`
Stop the animation.

#### `setSpeed(newValue)`
Set the new value of speed (animated)

#### `setAmplitude(value)`
Set the new value of amplitude (animated)

## Projects/examples that uses this script

* [The Capitol - The Official Government of Panem (Hunger Games Mockingjay Part 1 website)](http://www.thecapitol.pn/)
* [http://blog.kidliaa.com/demo/siri%20wave/](http://blog.kidliaa.com/demo/siri%20wave/ )

## Some math

![image](https://cloud.githubusercontent.com/assets/839700/3263201/224d98ec-f26f-11e3-971c-1e87f66a212f.JPG)
