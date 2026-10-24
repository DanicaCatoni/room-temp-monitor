# room-temp-monitor

Arduino temperature monitor with a 16x2 I2C LCD, audio/visual alarms and a 3D-printed OnShape enclosure

Arduino firmware in C++ for a room temperature monitor. It shows the live temperature on a 16x2 I2C LCD and triggers sound and light alarms when the reading leaves a set range. I designed and 3D-printed the enclosure in OnShape.

**Personal hardware project, Jan – May 2026**

## Features
- Continuous temperature readout on a 16x2 I2C LCD
- Configurable safe range with audio and visual alarms outside it
- Custom 3D-printed enclosure designed in OnShape

## Hardware
| Part | Notes |
|---|---|
| Arduino (AVR) board | e.g. Uno / Nano |
| Temperature sensor | _add model_ |
| 16x2 LCD with I2C backpack | I2C address _0x27 / 0x3F_ |
| Buzzer and LED | Alarm outputs |

## Wiring
_Add a wiring table or diagram (`docs/images/wiring.png`)._

## Build and upload
1. Open `firmware/` in the Arduino IDE (or PlatformIO).
2. Install the LCD I2C library listed at the top of the sketch.
3. Set the alarm thresholds, then upload.

## Repository layout
```
firmware/      Arduino sketch (C++)
enclosure/     OnShape export (STEP/STL) and link to the CAD document
docs/images/   photos and wiring diagram
```

## Author
Danica Catoni, Boston University · [danicacatoni.github.io](https://danicacatoni.github.io)
