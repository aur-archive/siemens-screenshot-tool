# Maintainer: Gudvin-t
# Contributor: Azq2

pkgname=siemens-screenshot-tool
pkgver=1.0
pkgrel=1
pkgdesc='Take screenshot for Siemens Mobile'
arch=('i686' 'x86_64')
url='http://team-sc.ru/viewtopic.php?p=158063'
depends=('gtk3' 'gtkmm')
license=("GNU LGPL")
source=("sst-${pkgver}.tar.gz")
md5sums=('eda547ffc8241489124d2cb8664f27a5')

build() {
  cd ${srcdir}/${pkgname}-${pkgver}
  make
}

package() {
  cd ${pkgname}-${pkgver}

  mkdir -p ${pkgdir}/usr/bin

  make install PREFIX=${pkgdir}/usr
}

