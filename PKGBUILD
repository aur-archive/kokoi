# Maintainer: Alessandro Di Martino <aledimax@gmail.com>

pkgname=kokoi
pkgver=LATEST
pkgrel=1
pkgdesc="Configurable markup file watcher, previewer and converter."
arch=('any')
url="https://github.com/zeis/kokoi"
license=('MIT')
depends=('nodejs' 'markdown')
makedepends=('gcc' 'make')
provides=('kokoi')

package() {
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p $_npmdir
  cd $_npmdir
  npm install --user root -g --prefix "$pkgdir/usr" $pkgname
}
