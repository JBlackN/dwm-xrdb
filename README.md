dwm-xrdb
========

Patch for [DWM](https://dwm.suckless.org/) allowing to load colors from [X resources](https://en.wikipedia.org/wiki/X_resources) at run time.

Installation and usage
----------------------

```bash
git clone git://git.suckless.org/dwm
cd dwm
git checkout tags/6.2 -b v6.2

git apply dwm-xrdb-6.2.diff

vi config.h                           # Edit config if needed.

make
```

X resources used:

```bash
dwm.normbordercolor
dwm.normbgcolor
dwm.normfgcolor
dwm.selbordercolor
dwm.selbgcolor
dwm.selfgcolor
```

Example Xresource string: `dwm.normbgcolor: #002b36`.

Default key to reload is `Mod+F5`.
