# Coordinate Converter

[中文](README.md)

A pure front-end static web tool for converting 2bulu favorite coordinates into Amap (Gaode) markers. It supports reverse geocoding, KML / CSV export, and copying Amap URI links.

## Usage

1. Clone or download this repository.
2. Open `amap.html` directly in your browser.
3. Enter your Amap JS API Key at the top of the page (stored locally in browser `localStorage` only; click "清除" to remove it; hover "如何获取 Key？" for steps to get one).
4. Paste coordinates on the left, one per line: `latitude,longitude` or `longitude,latitude`, optionally followed by a name.

Example:

```text
33.672416, 103.490997
39.908823, 116.397470 Tiananmen
```

## Get an Amap JS API Key

- Go directly to the Amap console [Application Management page](https://console.amap.com/dev/key/app).
- Register / log in, click "创建新应用" (Create Application), then click "添加 Key" (Add Key) on the application.
- Choose **Web 端 (JS API)** as the service platform to get a Key.

Your Key is stored only in your browser locally; it is not uploaded to any server or repository.

## Features

- Auto-detect latitude/longitude order (if the first number is greater than 90, it is treated as longitude).
- Supports WGS84 (default) / GCJ-02 / BD09 input coordinate systems, automatically converted to Amap's GCJ-02 during parsing.
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
