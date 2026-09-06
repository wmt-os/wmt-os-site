# Community

Use [Discussions](https://github.com/orgs/wmt-os/discussions) for help, device reports, and anything that isn't a concrete bug. Reproducible bugs go to the issue tracker of the repository they concern (see Development below).

WMT OS is currently a solo project, so responses may take time. Please don't let that stop you from participating.

## Contact

Security concerns and direct inquiries go to [root@wmt-os.org](mailto:root@wmt-os.org).

## Development

### Repositories

Everything lives on GitHub under the [wmt-os](https://github.com/wmt-os) organization:

- **[wmt-os](https://github.com/wmt-os/wmt-os)**: The build system that produces the images.
- **[linux-wmt](https://github.com/wmt-os/linux-wmt)**: The kernel fork powering the platform.
- **[xf86-video-wmt](https://github.com/wmt-os/xf86-video-wmt)**: The 2D-accelerated X.org video driver.
- **[wmt-os-dist](https://github.com/wmt-os/wmt-os-dist)**: The publishers and package recipes.
- **[wmt-os-site](https://github.com/wmt-os/wmt-os-site)**: This website.

### Kernel

The kernel fork tracks the `6.12.y` LTS branch. Development focuses on modernizing the SoC's hardware support. Recent work added new DRM/KMS, DMA engine, ASoC, CCF, serio, and battery drivers.

### Package repository

Every image is preconfigured with the signed WMT OS APT repository at [apt.wmt-os.org](//apt.wmt-os.org/), pinned above Debian. It delivers the kernel and other packages.

```
Suite         trixie
Component     main
Architecture  armel
Signing key   95E6 36EE F152 8AB3 5C1C  03F7 C88A B208 97CC 3653
```
