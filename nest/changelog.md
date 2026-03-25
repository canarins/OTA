# Canarin Nest — Firmware Changelog

## v1.0.1 (2026-03-25)

- GPS relay from Android app (USB serial `GPS_SET:` + REST `POST /api/location`)
- Responsive dashboard (adaptive grid, mobile-friendly touch targets)
- OTA firmware push via Birdhouse (Code 2 with `ota_url:`)
- LittleFS OTA endpoint (`POST /update-fs`)
- WiFi reset via REST (`POST /api/wifi/reset`)
- OTA check/apply REST endpoints (`/api/ota/check`, `/api/ota/apply`)

## v1.0.0 (2026-03-23)

Initial release.

- PMS7003, BME280, SGP40 sensor suite
- Wi-Fi captive portal provisioning
- Local web dashboard (`canarin.local`) with real-time data, AQI ring, 30-min history
- UDP Nano protocol communication (port 60004)
- 96-day offline circular buffer on LittleFS
- RGB LED status indicator (10 states)
- USB serial interface with CSV streaming and phone app commands
- ArduinoOTA local network updates
- Cloud OTA via GitHub manifest (`canarins/OTA`)
