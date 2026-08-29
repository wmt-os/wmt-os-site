# Development

Development happens on GitHub under the [wmt-os](https://github.com/wmt-os) organization:

- **[wmt-os](https://github.com/wmt-os/wmt-os)**: The build system that produces the images.
- **[linux-wmt](https://github.com/wmt-os/linux-wmt)**: The kernel fork powering the platform.
- **[xf86-video-wmt](https://github.com/wmt-os/xf86-video-wmt)**: The 2D-accelerated X.org video driver.
- **[wmt-os-dist](https://github.com/wmt-os/wmt-os-dist)**: The publishers and package recipes.

Report bugs to the repository they concern. Everything else goes to [Community](community.html).

## Kernel

The kernel fork tracks the `6.12.y` LTS branch. Active development continues to modernize the SoC's hardware support, with recent work bringing new DRM/KMS, DMA engine, ASoC, CCF, Serio, and battery drivers to the platform.

## Package repository

Every image is preconfigured with the signed WMT OS APT repository at [apt.wmt-os.org](https://apt.wmt-os.org/), pinned above Debian. It delivers the kernel and other packages.

```
Suite         trixie
Component     main
Architecture  armel
Signing key   95E6 36EE F152 8AB3 5C1C  03F7 C88A B208 97CC 3653
```
