# Frontear's Repository
A personally maintained Arch Linux repository for some of my most used packages.

This repository was made out of frustration with maintainers on the Arch User Repository
providing broken packages, incomplete program files, too many or missing dependencies, and a broken build pipeline.

The main purpose of the PKGBUILDs here are to "just work", using as similar of a build pipeline as possible to what the sources recommend.

## How to use?
Add this github repository as a custom package repository in your `/etc/pacman.conf`:

```conf
[frontear]
Server = https://raw.githubusercontent.com/Frontear/packages/main/x86_64
```

Then, import my gpg key [BCB5CEFDE22282F5](https://gist.github.com/Frontear/e927f66b37db9fd8a1be18fea02d0cf1):

```console
# pacman-key --add /path/to/frontear.gpg
# pacman-key --lsign-key BCB5CEFDE22282F5
```

Finally, run `pacman -Syu` to refresh local databases and install as you would a normal arch package.

## License
All code in this repo (the binaries and PKGBUILD scripts) are subject to the GNU General Public License v3.0. Please be mindful of this when forking, downloading, and redistributing.

Please also note that the programs provided via these scripts, and the overarching repository are **NOT** subject to the above license. They possess their own licenses, which are either packaged with them or presented upon installing the package. Please be mindful of this when downloading, installing, and running these programs.
