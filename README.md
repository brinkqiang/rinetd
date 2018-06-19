# rinetd

## Intro
rinetd, port mapped tools

## Prerequisites

### Get the latest source code

To get the latest source code:

```bash
git clone https://github.com/brinkqiang/rinetd.git
pushd rinetd
yum install gettext gcc autoconf libtool automake make asciidoc xmlto c-ares-devel libev-devel

sudo libtoolize && sudo aclocal && sudo autoheader && sudo autoconf && sudo automake --add-missing

sh configure
make
make install
popd
```
### config
```
vim /usr/local/etc/rinetd.conf
```
### run
```
rinetd -c /usr/local/etc/rinetd.conf
```

## License
rinetd, by Thomas Boutell and Sam Hocevar. Released under the terms
of the GNU General Public License, version 2 or later.

This program is used to efficiently redirect connections from one IP
address/port combination to another. It is useful when operating virtual
servers, firewalls and the like.

To build under Unix, run `./bootstrap` to create the configuration
files, then `./configure` to create the build files, and then type
`make` to build rinetd. To install, type `make install` as root.

For documentation run `make install`, then type `man rinetd` for
details. Or, read `index.html` in your browser.

