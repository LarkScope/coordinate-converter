# Amap Favorites Converter

[中文](README.md)

A pure front-end static web tool for converting 2bulu favorite coordinates into Amap (Gaode) markers. It supports reverse geocoding, KML / CSV export, and copying Amap URI links.

## Usage

1. Clone or download this repository.
2. Open `amap.html` directly in your browser.
3. Enter your Amap JS API Key at the top of the page (stored locally in browser `localStorage` only).
4. Paste coordinates on the left, one per line: `latitude,longitude` or `longitude,latitude`, optionally followed by a name.

Example:

```text
33.672416, 103.490997
39.908823, 116.397470 Tiananmen
```

## Get an Amap JS API Key

- Visit [Amap Open Platform](https://lbs.amap.com/).
- Register / log in, then go to Console → Application Management → My Applications → Add Key.
- Choose **Web (JS API)** to get a Key.

Your Key is stored only in your browser locally; it is not uploaded to any server or repository.

## Features

- Auto-detect latitude/longitude order (if the first number is greater than 90, it is treated as longitude).
- Display all points on the map.
- Batch reverse geocoding to get address names.
- Export KML (can be opened in Google Earth, etc.).
- Export CSV.
- Copy all Amap URI links.

## Files

- `amap.html` — The complete tool page (HTML + CSS + JavaScript).
- `LICENSE` — MIT License.

## License

MIT
