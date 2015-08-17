# Maintainer: Alexander Duscheleit <jinks@archlinux.us>
pkgname=python2-colorama
pkgver=0.3.3
pkgrel=1
pkgdesc="Python API for cross-platform colored terminal text."
arch=('any')
url="http://pypi.python.org/pypi/colorama"
license=('BSD')
depends=('python2')
source=(http://pypi.python.org/packages/source/c/colorama/colorama-$pkgver.tar.gz)
md5sums=('a56b8dc55158a41ab3c89c4c8feb8824')

build() {
  cd "$srcdir/colorama-$pkgver"

  python2 setup.py build
}

package() {
  cd "$srcdir/colorama-$pkgver"

  python2 setup.py install --root=$pkgdir --optimize=1
}

# vim:set ts=2 sw=2 et:
