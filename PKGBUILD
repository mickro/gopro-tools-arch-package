# Maintainer: Mickael Foucaux <mickael.foucaux@gmail.com>
pkgname=gopro-tools
pkgver=1
pkgrel=1
pkgdesc="Useful tool set for post production"
arch=('any')
url="https://github.com/KonradIT/gopro-linux"
license=('GPL3')
groups=('gopro')
depends=('mencoder' 'ffmpeg' 'imagemagick')
source=('https://raw.githubusercontent.com/KonradIT/gopro-linux/master/gopro')
md5sums=('9b056dccbe56c509ddfa1e673c584fad')

package() {
  install -D -m755 $srcdir/gopro $pkgdir/usr/bin/gopro
}
