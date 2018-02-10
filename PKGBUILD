# Maintainer: manuel (see forum.antergos.com)

pkgdesc="A simple HTTP based file server for home users on local networks."
pkgname=filedrawer
pkgver=1.15
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash' 'yad' 'ufw' 'gksu' 'python')  # python 3 required
source=("$url/raw/master/$pkgname-$pkgver")
sha512sums=('f7c1e9d9f5ac6ab487ca791b27cbb308ec956f44f29df6316422a6927b65ea2c62c6917905670b66907b44fa403f37bdbfc5dd34f4d3670260d75e78765156f7')

package() {
  cd $srcdir
  install -Dm555 $pkgname-$pkgver $pkgdir/usr/bin/$pkgname
}
