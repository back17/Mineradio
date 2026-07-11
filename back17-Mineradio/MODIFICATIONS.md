# Modifications

This working tree is a modified version of [XxHuberrr/Mineradio](https://github.com/XxHuberrr/Mineradio).

- Original project copyright: Copyright (C) 2026 XxHuberrr.
- License: GNU General Public License v3.0. The original `LICENSE` and `NOTICE.md` are retained.
- Upstream source snapshot: `6b130103f759e5dcd1e133700071c8216b8fa5a6`.
- Modified repository: `back17/Mineradio`.
- Modified release version: `1.1.1-weather.1`.
- This file records changes made after that upstream snapshot.

## 2026-07-11

- Replaced the Home construction placeholder with a weather forecast panel that follows the existing Mineradio glass UI.
- Made the weather panel open a detailed forecast view.
- Added city search, IP-based location, refresh, and weather-radio actions to the detailed view.
- Added eight current-weather metrics, a 24-hour forecast, and a 7-day forecast with precipitation, wind, sunrise, sunset, pressure, visibility, and UV data.
- Kept the compact Home view at six hourly entries and four daily entries.
- Extended the existing Open-Meteo weather endpoint instead of introducing a separate weather service.

Modified source files:

- `public/index.html`
- `server.js`
