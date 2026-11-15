# Data Format

## WAV File Specifications

| Property | Value |
|---|---|
| Format | WAV (PCM) |
| Sample rate | 44,100 Hz |
| Bit depth | 16-bit |
| Channels | Mono (1 channel) |
| Duration per file | 10 seconds (full dataset) / 2 seconds (preview) |
| Naming convention | `HHMMSS_xx.wav` (timestamp-based) |

## Class Labels

| Folder name | Label | Description |
|---|---|---|
| `leak_night` | Leak | Pipe leak signal recorded at night (no background traffic) |
| `leak_daytime_vehicle` | Leak | Pipe leak signal recorded during daytime with vehicle traffic |
| `no_leak` | No Leak | Baseline recording, no leak present |

## Recording Conditions

- **Pipe material**: PVC / HDPE
- **Pipe diameter**: 90–110 mm
- **Burial depth**: 30–31 cm
- **Sensor placement**: Ground surface directly above the pipe
- **Environment**: Urban area, Ho Chi Minh City, Vietnam

