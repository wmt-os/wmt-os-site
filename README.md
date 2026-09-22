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

The web host keeps a clone of this repository in the `builder` account, with a local `.git/hooks/post-merge` that rebuilds the site and rsyncs `public/` to the `webroot` account, so a deploy is a push here and a `git pull` there:

```sh
#!/bin/sh
set -e
ikiwiki --setup ikiwiki.setup
rsync -a --delete public/ webroot:wmt-os.org/
```

## License

MIT - see [LICENSE.md](LICENSE.md).
