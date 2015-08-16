# Maintainer: Lucas Hermann Negri <lucashnegri@gmail.com>

pkgname=lua-supernn
pkgver=0.6.0
pkgrel=1
pkgdesc="A simple binding of SuperNN[1] to Lua 5.1 / luajit"
arch=('i686' 'x86_64')
url="http://oproj.tuxfamily.org" 
depends=('supernn' 'lua51')
makedepends=('gcc' 'swig')
license=(LGPL)
source=("https://bitbucket.org/lucashnegri/$pkgname/downloads/$pkgname-$pkgver.tar.gz")
md5sums=("fcc7fb09154b91f266205dce8fb0ad4d")

build() { 
    cd "$srcdir/$pkgname-$pkgver"
    make
}

package() {
    cd "$srcdir/$pkgname-$pkgver"
    make install PREFIX=${pkgdir}/usr
}
