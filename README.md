# Map shortcode for Hugo

This shortcode embeds a GPX track on a map. It utilises the [Leaflet library](https://leafletjs.com).

## Usage:

1. Add this repo as a submodule: `git submodule add git@github.com:martinschneider/hugo-gpx-shortcode.git themes/gpx-shortcode`.
2. Add `gpx-shortcode` as a theme to your config: e.g. `theme = ["bare", "gpx-shortcode"]`
3. Configure the map layer and (optional) map attribution:

```
[params]
  mapLayer = "https://tile.thunderforest.com/outdoors/{z}/{x}/{y}{r}.png?apikey=..."
  mapAttribution = "Maps © <a href=\"http://www.thunderforest.com\">Thunderforest</a>, Data © <a href=\"http://www.openstreetmap.org/copyright\">OpenStreetMap contributors</a>"
```

4. Place your gpx files under `/static/gpx`.
5. Use the shortcode in your posts like this: `{{< gpx id="everest" >}}`. The `id` parameter is the filename without the `.gpx` extension.

Please refer to the [code](layouts/shortcodes/gpx.html) and the [Leaflet documentation](https://leafletjs.com/) for more details.

Please feel free to submit pull requests to improve this short code.