# leaflet-measure-distance [![NPM version][npm-image]][npm-url] [![NPM Downloads][npm-downloads-image]][npm-url]

Measure distances interactively on a leaflet map.

Adds a leaflet control which allows you to activate an interactive mode to measure and annotate distances on the map.

The default units are kilometers, however you can supply an arbitrary scale factor (from meters) and label to support your prefered units.

## Example use:

Default: `kilometers`:

```javascript
const map = new L.Map("map", {
  measureControl: {
    enabled: true,
  },
});
```

e.g.: `nautical miles`:

```javascript
const map = new L.Map("map", {
  measureControl: {
    enabled: true,
    unitLabel: "nm",
    unitFactor: 1852,
  },
});
```

e.g.: `meters`:

```javascript
const map = new L.Map("map", {
  measureControl: {
    enabled: true,
    unitLabel: "m",
    unitFactor: 1,
  },
});
```

For a demo see [here](http://onaci.github.io/leaflet.measure/example.html).

## License

CSIRO Open Source Software Licence Agreement (variation of the BSD / MIT License)

[npm-image]: https://badge.fury.io/js/leaflet-measure-distance.svg
[npm-url]: https://www.npmjs.com/package/leaflet-measure-distance
[npm-downloads-image]: https://img.shields.io/npm/dt/leaflet-measure-distance.svg
