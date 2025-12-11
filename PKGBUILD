pkgname=st-fb
pkgver=1.0
pkgrel=1
pkgdesc="-A simple virtual terminal emulator for X - Fryed Version"
url="https://github.com/fryedbiscuit/st"
arch=('i686' 'x86_64' 'armv7h' 'aarch64')
license=('MIT')
# options=(zipman)
depends=('libxft')
provides=('st')
conflicts=('st')

build() {
  make
}

package() {
  make PREFIX="${PREFIX:-/usr}" DESTDIR="$pkgdir" install
}
