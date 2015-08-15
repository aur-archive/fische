# Current Maintainer: Kozec <kozec at kozec dot com>

# Contributor: Anton Bazhenov <anton.bazhenov at gmail>
# Contributor: antisystem <antisystem@jabber.org>

pkgname=fische
pkgver=4.0.2
pkgrel=1
pkgdesc="A standalone music vizualisation application"
arch=('i686' 'x86_64')
url="http://26elf.at/"
license=('MIT')
depends=('freeglut' 'gcc-libs')
makedepends=('cmake')
source=("http://26elf.at/files/$pkgname-$pkgver.tar.xz")

build() {
  cd "$srcdir"/$pkgname-${pkgver}
  cmake . || return 1
  make
}

package() {
  cd "$srcdir"/$pkgname-${pkgver}
  mkdir -p "$pkgdir"/usr/bin || return 1
  cp fische "$pkgdir"/usr/bin || return 1
}

md5sums=('a152aebbb5b4fb573de7a70a53b2b5b8')
md5sums=('abc2d567d1252b7928448ee93580f9f6')
