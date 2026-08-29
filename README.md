# WMT OS Site

Website and documentation for [WMT OS](https://github.com/wmt-os/wmt-os), published at [wmt-os.org](https://wmt-os.org/).

The site is plain Markdown compiled to static HTML by [ikiwiki](https://ikiwiki.info/), with no JavaScript.

* `content/`: One Markdown file per page, changelog entries under `changelog/`, images under `images/`.
* `templates/`: The page frame and the changelog listing templates.
* `ikiwiki.setup`: The build configuration.

## Building

Requires: `ikiwiki libtimedate-perl`

```sh
ikiwiki --setup ikiwiki.setup
```

The site is written to `public/`.

## Deploying

The web host holds a clone of this repository and rebuilds from a local `.git/hooks/post-merge`, so a deploy is a push here and a `git pull` there:

```sh
#!/bin/sh
exec ikiwiki --setup ikiwiki.setup --set destdir=/home/webroot/wmt-os.org
```

## License

MIT - see [LICENSE.md](LICENSE.md).
