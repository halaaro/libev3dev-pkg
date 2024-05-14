# Maintainer: Aaron Haley <15240680+halaaro@users.noreply.github.com>
_project='ev3dev-c'
pkgname="libev3dev"
pkgver='0.6.5'
pkgrel=1
pkgdesc="$_project library and headers"
arch=('x86_64')
url="https://github.com/halaaro/$pkgname-pkg"
license=('MIT')
depends=()
makedepends=()
checkdepends=()
optdepends=()
provides=("$pkgname=0.6.5")
backup=()
options=('!strip' '!buildflags')
install=
changelog=
source=("$pkgname-$pkgver.tar.gz::https://github.com/halaaro/$_project/archive/refs/tags/v$pkgver.tar.gz")
sha256sums=('625f50a3aa2590949f8d61bae064a9b9e6996af921e7977669a64b0cf3445f37')

package() {
  cd "$srcdir/$_project-$pkgver"
  install source/ev3/ev3*.h -Dt "${pkgdir}/usr/include"
  install  lib/libev3dev-c.a -DT "${pkgdir}/usr/armv5tej/lib/libev3dev.a"
}
