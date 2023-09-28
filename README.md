# Frontear's Repository
My personal repository containing Arch Linux PKGBUILD's for software I use often. This was made out of frustration from the AUR and official repos having incorrect packages, wildly unnecessary dependency additions and flawed building process, or straight up missing features.

## How to use?
Add this github repository as a custom package repository in your `/etc/pacman.conf`:

```conf
[frontear]
SigLevel = Optional TrustAll
Server = https://raw.githubusercontent.com/Frontear/packages/main/x86_64
```

Then, just run `pacman -Syu` to refresh local databases.
