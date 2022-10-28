# Maintainer: Philip Müller <philm[at]manjaro[dot]org>
# Maintainer: Bernhard Landauer <bernhard[at]manjaro[dot]org>

# Arch credits:
# Pierre Schmitz <pierre@archlinux.de>

pkgname=manjaro-keyring
pkgver=20221028
pkgrel=2
pkgdesc="Manjaro PGP keyring"
arch=('any')
url="https://manjaro.org"
license=('GPL')
groups=('base-devel')
depends=('pacman')
install="${pkgname}.install"
source=('Makefile'
        'manjaro.gpg'
        'manjaro-revoked'
        'manjaro-trusted')
sha256sums=('c5a0ede3f665150f2d53a4e4c4b6f82abd108a2a6ff11b406a64d5b8bc6583dd'
            '31d7e0f8c1741fa4f8d7cc7873539199c568d73e539483844b363ea539f90a42'
            '3e909acd91874ea0b0dc7655f8ab549a2ea4cbae5ab6a19b08f71a654a728932'
            'ff6f35edd535703cd8e62adfb4b03e79005a04230da76d7ea8c394bb74bce4c6')

package() {
  make DESTDIR="${pkgdir}" install
}
