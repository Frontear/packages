# Frontear's Repository
My personal repository containing Arch Linux PKGBUILD's for software I use often. This was made out of frustration from the AUR and official repos having incorrect packages, wildly unnecessary dependency additions and flawed building process, or straight up missing features.

## How to use?
Add this github repository as a custom package repository in your `/etc/pacman.conf`:

```conf
[frontear]
Server = https://raw.githubusercontent.com/Frontear/packages/main/x86_64
```

Then, import my gpg key: [BCB5CEFDE22282F5](https://gist.github.com/Frontear/e927f66b37db9fd8a1be18fea02d0cf1):

```
# pacman-key --add /path/to/frontear.gpg
# pacman-key --lsign-key BCB5CEFDE22282F5
```

Finally, run `pacman -Syu` to refresh local databases and install as you would a normal arch package.

## License
All code in this repo (the binaries and PKGBUILD scripts) are subject to the GNU General Public License v3.0. Please be mindful of this when forking, downloading, and redistributing.
Please also not that the programs provided via these scripts, and the overarching repository are **NOT** subject to the above license. They possess their own license, which are either packaged with them or presented upon installing the package. Please be mindful of this when downloading, installing, and running these programs.
