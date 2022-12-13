# GPX shortcode for Hugo

This shortcode displays GPX tracks on a map using the [Leaflet library](https://leafletjs.com).

## Usage

1. Add this repo as a submodule: `git submodule add git@github.com:martinschneider/hugo-gpx-shortcode.git themes/gpx-shortcode`.
2. Add `gpx-shortcode` as a theme to your config: e.g. `theme = ["bare", "gpx-shortcode"]`
3. Use the shortcode in your posts like this: `{{< gpx "everest.gpx" >}}`.


### Configuration (optional)
```
[params.gpx]
  leafletJS = "https://cdnjs.cloudflare.com/ajax/libs/leaflet/1.8.0/leaflet-src.min.js"
  leafletGpxJS = "https://cdnjs.cloudflare.com/ajax/libs/leaflet-gpx/1.7.0/gpx.min.js"
  leafletCSS = "https://unpkg.com/leaflet@1.8.0/dist/leaflet.css"
  trackColors = ["blue", "darkblue", "purple"]
  layers = [ { url = "https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", attribution = "(c) <a href="https://www.openstreetmap.org/copyright">OpenStreetMap</a> contributors" } ]
```

Please refer to the [code](layouts/shortcodes/gpx.html) and the [Leaflet documentation](https://leafletjs.com/) for more details.

## Demo
I use this shortcode on [my blog](https://www.grainsofsand.at).


## Support
Please feel free to submit pull requests to improve this shortcode.