# For users of the Archlinux family

dnscrypt-proxy Git version configured with support for plugins and domains blacklist.

# Installation on Archlinux

For the use of the plugins it is necessary to add the option "options" with the parameter "libtool" in the PKGBUILD file, like this: 

> * options=(libtool)

After this, you need to build the package again with the makepkg command. However, you can install dnscrypt-proxy in two ways:

* The first, by installing the stable version of the package, like this:    

    > sudo pacman -S dnscrypt-proxy 

* The second, by installing the git version of the package, like this:

    > yaourt -S dnscrypt-proxy-git

There is a difference between both packages, the git version in AUR is ready and configured for use with the plugins and the script for to generate blacklist domains. However, if you want to install the stable version, there is a version in [github](https://github.com/FixedTorres/dnscrypt-proxy) configured for to use plugins and the script for to generate blacklist domains.

Once this is done, all files with .la extension are located in the `/usr/lib/dnscrypt-proxy/` directory. Without adding `options=(libtool)`, all files with .la extension disappears.

**AUR:** https://aur.archlinux.org/packages/dnscrypt-proxy-git/

**For more information, see:** https://github.com/jedisct1/dnscrypt-proxy/wiki
