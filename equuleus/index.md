---
layout: home
title: Unofficial VyOS `equuleus` Package Repository
---
Since the maintainers of the VyOS project have [decided](https://blog.vyos.io/community-contributors-userbase-and-lts-builds) that they won't permit external access to their own package repositories anymore, I've set up my own unofficial one.

### Using with `vyos-build`

Run the `configure` script from the [`vyos-build` repository](https://github.com/vyos/vyos-build/blob/equuleus), passing the --vyos-mirror argument. Then run `sudo make iso`:

```
sudo ./configure --architecture amd64 --build-by "j.randomhacker@vyos.io" --vyos-mirror "[trusted=yes] {{ site.url }}/vyos-pkg/equuleus/deb"
sudo make iso
```

## How to contribute?

Please contribute changes and bug reports in the relevant repository above.

Have a security issue? Please email [Matthew](mailto:matthew@kobayashi.au) with details.

Have your own action? Please create a [pull request on this repository](https://mattkobayashi.github.io/vyos-pkg.github.io/pulls).