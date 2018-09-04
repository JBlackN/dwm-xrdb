dwm-xrdb
========

Patch for [DWM](https://dwm.suckless.org/) allowing to load colors from [X resources](https://en.wikipedia.org/wiki/X_resources) at run time.

Installation and usage
----------------------

```bash
git clone git://git.suckless.org/dwm
cd dwm
git checkout tags/6.1 -b v6.1

git apply dwm-xrdb-6.1.diff

rm config.h                           # !!! CAREFUL !!!
make config.h
vi config.h                           # Fill in path to your .Xresources file.

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

Default key to reload is `Mod+F5`.
