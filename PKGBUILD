# Author: Appcelerator, Inc. <npmjs@appcelerator.com>
# Maintainer: tonylukasavage <anthony.lukasavage@gmail.com>
# Maintainer: cb1kenobi <chris@cb1inc.com>
# Maintainer: appcelerator <npmjs@appcelerator.com>
_npmname=titanium
_repo="git://github.com/appcelerator/titanium.git"
pkgname=nodejs-titanium-git
pkgver=3.4.0_dev
pkgrel=1
pkgdesc="Appcelerator Titanium Command line (last dev version)"
arch=(any)
url="https://github.com/appcelerator/titanium"
license=(Apache Public License v2)
depends=('nodejs')
conflicts=('nodejs-titanium')
provides=('nodejs-titanium')
optdepends=()

package() {
  cd $srcdir
  local _npmdir="$pkgdir/usr/lib/node_modules/"
  mkdir -p "$_npmdir"
  cd "$_npmdir"
  npm install -g --prefix "$pkgdir/usr" $_repo 
}
