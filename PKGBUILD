# Maintainer: Mickael Foucaux <mickael.foucaux@gmail.com>
pkgname=gopro-tools-git
pkgver=1.0.r0.g5c6bd4e
pkgrel=1
pkgdesc="Useful tool set for post production"
arch=('any')
url="https://github.com/KonradIT/gopro-linux"
license=('GPL3')
groups=('gopro-git')
conflicts=('gopro-tools')
depends=('mencoder' 'ffmpeg' 'imagemagick')
source=('git+https://github.com/KonradIT/gopro-linux.git')
md5sums=('SKIP')

pkgver() {
  cd gopro-linux
  git describe --long --tags | sed 's/\([^-]*-g\)/r\1/;s/-/./g'
}

package() {
  install -D -m755 "$srcdir/gopro-linux/gopro" "$pkgdir/usr/bin/gopro"
}
