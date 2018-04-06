# Git version of Dnscrypt for the Archlinux family

Git version of dnscrypt-proxy configured with plugin support and domain blacklist.

# Installation on Archlinux

For the use of the plugins it is necessary to add the option "options" with the parameter "libtool" in the file PKGBUILD, as well: 

> * options=(libtool)

After that, you need to rebuild the package with the command makepkg:

* [fixedtorres@linuxero ~]$ makepkg

You can also download the version of this repository and run the previous makepkg command. This version git is ready and configured for use with the plugins and the script for generating blacklisted domains. However, if you want to install the stable version, there is a version in [github](https://github.com/FixedTorres/dnscrypt-proxy) configured to use plugins and the script to generate blacklisted domains.

Once this is done, all files with .la extension are located in the `/usr/lib/dnscrypt-proxy/` directory. Without adding `options=(libtool)`, all files with .la extension disappears.

**GIT Repository** https://github.com/dyne/dnscrypt-proxy
