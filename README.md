MausamPK

Fast, bilingual (English and Urdu) weather for cities and towns across Pakistan.

Live site: https://your-domain.com

Features
Current conditions: temperature, feels-like, humidity, wind, pressure, UV index, rain chance, sunrise and sunset
Next 24 hours hourly forecast and 7-day forecast with temperature range bars
51 built-in cities plus a search box for any city or town in Pakistan (Open-Meteo geocoding)
"My location" button using the browser Geolocation API
English and Urdu interface with automatic RTL layout (Noto Nastaliq Urdu)
Dynamic sky theme (clear, night, cloudy, rain, storm, snow) with custom inline SVG icons
Responsive, light/dark mode, keyboard-friendly focus styles
Remembers last city and language in localStorage
Single static file, no framework, no API key
Data source

Weather data comes from the Open-Meteo Forecast and Geocoding APIs.

Note: Open-Meteo's free tier is intended for non-commercial use. If you run ads or otherwise monetize the site, review their terms and use a commercial plan or another provider.

Forecasts are model estimates and are not an official warning service. Follow the Pakistan Meteorological Department for severe weather alerts.

Project structure
.
├── index.html   # entire site: markup, styles and scripts
└── ads.txt      # Google AdSense authorized sellers file
Run locally
bash
git clone https://github.com/your-username/mausampk.git
cd mausampk
npx serve .

Open the printed local URL. An internet connection is required for live data.

Deploy

Any static host works (Netlify, Cloudflare Pages, GitHub Pages, Vercel). No build command is needed.

Customize

Add a city: in index.html, find const C=[ and append an entry:

js
['Okara','اوکاڑہ',30.81,73.45]   // English name, Urdu name, latitude, longitude

Branding and ads: replace MausamPK, the contact email and the AdSense publisher ID (ca-pub-...) in index.html, and update ads.txt.

Roadmap
 Dedicated page per city (/lahore-weather) for search visibility
 Air quality (AQI) panel
 Weather alerts and monsoon section
 °C / °F toggle
Contributing

Issues and pull requests are welcome. Please open an issue first for larger changes.# MausamPk.com
