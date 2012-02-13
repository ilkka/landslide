# Maintainer: Ilkka Laukkanen <ilkka.s.laukkanen@gmail.com>
pkgname=landslide
pkgver=1.0.1
pkgrel=1
pkgdesc="Generate html5 slideshow from Markdown or reStructuredText sources"
arch=(any)
url="http://github.com/adamzap/landslide"
license=('Apache License')
depends=('python2' 'python2-pygments' 'python2-markdown' 'python2-jinja' 'docutils')
makedepends=('python2-distribute')
optdepends=('princexml')
source=(http://pypi.python.org/packages/source/l/$pkgname/$pkgname-$pkgver.tar.gz)
md5sums=('199cdbd332c15f4771130abc9f95d1f2')

build() {
  cd "$srcdir/$pkgname-$pkgver"

  python2 ./setup.py build
}

package() {
  cd "$srcdir/$pkgname-$pkgver"

  python2 ./setup.py install --prefix=/usr/ --root=$pkgdir/
}

# vim:set ts=2 sw=2 et:

