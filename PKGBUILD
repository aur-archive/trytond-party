# Maintainer: Robin Baumgartner <robin@baumgartners.ch>
pkgname=trytond-party
_pkgname=trytond_party
pkgver=3.4.1
_pkgdir=3.4
pkgrel=1
pkgdesc="The party module of the Tryton application platform"
arch=('any')
url='http://www.tryton.org/'
license=('GPL3')
groups=('trytond-modules')
depends=('trytond>=3.4' 'trytond-country>=3.4')
makedepends=('python2-distribute')
source=("http://downloads.tryton.org/$_pkgdir/$_pkgname-$pkgver.tar.gz")
md5sums=("7a27d801a1d2cb4f8ef1c934c64e133c")

build() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py build
}

package() {
  cd $srcdir/$_pkgname-$pkgver
  python2 setup.py install --root=$pkgdir
}