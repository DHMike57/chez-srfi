# Maintainer: shiliang <shiliang2008@msn.com>

pkgname=chez-srfi
_pkgname=chez-srfi
pkgdesc='SRFI for ChezScheme'
pkgver=1.1
pkgrel=1
arch=('any')
url='https://github.com/shih-liang/chez-srfi.git'
license=('MIT')
depends=('chez-scheme')

source=( ${_pkgname}-${pkgver}-${pkgrel}.tar.gz::https://github.com/shih-liang/chez-srfi/archive/refs/tags/v${pkgver}.tar.gz)
md5sums=('SKIP')
provides=('chez-srfi')

build(){
  cd ${_pkgname}-${pkgver}
  make CHEZ=scheme
}
package(){
  cd ${_pkgname}-${pkgver}
  make install CHEZ=scheme PREFIX=${pkgdir}/usr
}
