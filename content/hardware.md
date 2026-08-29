# Hardware

These netbooks were sold under many brands, with boards that differ in audio codec, battery, and panel. The models below are known to work.

| Model                  | Display          | Audio codec       |
| ---------------------- | ---------------- | ----------------- |
| Sylvania SYNET07526    | 7 inch 800x480   | VT1612A or VT1613 |
| Sylvania SYNET7WID     | 7 inch 800x480   | VT1613            |
| JAY-tech Jay-Book 9901 | 7 inch 800x480   | VT1613            |
| EPC-1026               | 10 inch 1024x600 | WM9715L           |

Early Sylvania units are labeled SmartBook, later ones Netbook.

## Supported

| Component                     | Notes                                           |
| ----------------------------- | ----------------------------------------------- |
| Display                       | Built-in LCD panel, resolution auto-detected    |
| Backlight                     | PWM brightness control                          |
| Graphics acceleration, kernel | DRM/KMS driver with 2D and console acceleration |
| Graphics acceleration, X.org  | 2D-accelerated video driver with VSync          |
| Built-in audio                | Headphone and speaker output                    |
| Keyboard and touchpad         | Built-in PS/2 controller                        |
| SD card                       | Built-in SD/MMC controller                      |
| Wi-Fi                         | Internal USB adapter                            |
| USB peripherals               | Keyboards, mice, audio, storage, and networking |
| Battery monitoring            | Self-calibrating voltage-based estimation\*     |

\* VT1613 and VT1612A boards. WM9715L boards are not yet supported.

## Planned

| Component                 | Notes                                      |
| ------------------------- | ------------------------------------------ |
| Video decoder, JPEG/MJPEG | Dedicated decode engine for video playback |
| Video scaler              | Hardware scaling engine                    |

## Unsupported

| Component        | Notes                              |
| ---------------- | ---------------------------------- |
| Internal storage | NAND flash controller inaccessible |

## Unlisted models

Other WM8505 netbooks are likely compatible. Windows CE identifies the processor as ARM-WM8505. If yours is not listed, try it and post a [device report](community.html) with the result, even if everything just works.
