# -I4cortexComponents
A module that adds components to the Perspective module.
# Liquid-Chart

## Description

The Liquid Chart component is a versatile tool for visualizing liquid levels in tanks, providing you with the flexibility to customize various aspects of the chart.

<img src="Liquid-Chart.gif" alt="CLiquid-Chart" width="100%" />


## Properties

Here are the available properties for the Liquid Chart component:

| Property       | Type     | Default | Affects                            |
| -------------- | -------- | ------- | ---------------------------------- |
| `value`        | `number` | 0       | Value of your liquid level        |
| `max`          | `number` | 100     | Maximum level of your tank         |
| `isPercentage` | `boolean`| true    | If true, displays tank level in %  |
| `unit`         | `string` | "liter" | Appears when `isPercentage` is set to `false` |
| `formatt`      | `string` | "##"    | Format your displayed number       |
| `shape`        | `string` | "circle"| Tank shape (can be 'circle' or 'rect', etc.) |
| `outline`      | `object` | `{}`    | Customize outline style            |
| `liquid-style`| `object` | `{}`    | Customize liquid style             |
| `wave`         | `object` | `{}`    | Customize wave length and count    |
| `statistic`    | `object` | `{}`    | Customize label style              |
| `sizing`       | `object` | `{}`    | Customize chart sizing             |


## Example

```json
{
  "value": 80,
  "max": 100,
  "isPercentage": false,
  "unit": "liter",
  "formatt": "##.##",
  "shape": "circle",
  "outline": {
    "border": 1,
    "color": "",
    "distance": 1
  },
  "liquid-style": {
    "fill": "#8DBEE7",
    "lineDash": [
      0,
      0
    ],
    "lineWidth": 1,
    "shadowBlur": 10,
    "shadowColor": "",
    "strokeOpacity": 1,
    "shadowOffsetX": 5,
    "shadowOffsetY": 5,
    "stroke": "#87B1D3"
  },
  "wave": {
    "count": 3,
    "length": 122
  },
  "statistic": {
    "content": {
      "style": {
        "fill": "#000",
        "fontSize": 22,
        "lineWidth": 2,
        "opacity": 1,
        "shadowBlur": 1,
        "shadowColor": "#000"
      }
    }
  },
"sizing": {
  "autoFit": true,
  "radius": 1,
  "height": 400,
  "width": 400
}
}

## license

[MIT License](https://opensource.org/licenses/MIT)
