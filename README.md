# Simple-Wine-Building-Bot
[wine](https://www.winehq.org/), [wine-staging](https://github.com/wine-staging/wine-staging), [wine-pba](https://github.com/acomminos/wine-pba) download, patch, build, install script

Work on **Fedora**, other distor may work if have good **multilib** support. NOT the **chroot** way.

**Feature**
* Support custom patch for wine
* Support custom patch for wine-staging
* Support custom patch for wine-pba

**Change**
* 0.6.1: add support for pba-firerat
* 0.7.0: add optimize native cpu option

**Usage**
* Read script comment carefully
* Modify `# build setting` section 
* Modify `# setup your custom patch here` section, if you want to use some custom patches.

* Get more patches from [PKGBUILDS](https://github.com/Tk-Glitch/PKGBUILDS/tree/master/wine-tkg-git)
* Use winedepgen to generate wine runtime/build dependency package list on **Fedora 30**, install these packages manually to save download time.

**Tips for building wine with esync**
* Treat esync release as custom patch: extract esync.tgz to `wine_patch_dir`
* set `selector` to `'commit'`
* set `wine_commit` to esync rebased against hash
