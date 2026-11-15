# Data Collection Protocol

## Equipment

- Custom-built acoustic sensor based on **Raspberry Pi**
- Sensor type: hydrophone / MEMS microphone
- Sampling performed via onboard ADC at 44,100 Hz
- Files recorded as continuous 10-second WAV segments

## Field Procedure

1. Sensor placed on ground surface above buried pipe
2. Recording triggered manually or via scheduled timer
3. Ground truth annotated based on valve state (pump ON = Leak possible, pump OFF = No Leak)
4. Night sessions used to minimize vehicle noise interference
5. Daytime sessions intentionally captured vehicle pass-by events

## Session Dates

| Date | Depth | Condition |
|---|---|---|
| 2026-06-26 | — | Baseline noise capture |
| 2026-07-17 | 30 cm | Quiet, day |
| 2026-07-18 | 30 cm | Noisy (gravel + sand) |
| 2026-07-20 | — | Follow-up |
| 2026-07-21 | — | Night session |

