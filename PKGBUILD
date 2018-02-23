# Maintainer: manuel (see forum.antergos.com)

pkgdesc="A simple HTTP based file server for home users on local networks."
pkgname=filedrawer
pkgver=0.1.18
pkgrel=1
url="https://github.com/manuel-192/$pkgname"
arch=('any')
license=('GPL3')
depends=('bash' 'yad' 'ufw' 'gksu')
source=(
  "$url/raw/master/$pkgname-$pkgver"
  "$url/raw/master/$pkgname.desktop"
)
sha512sums=(
  'a5011b0acca99952c1879c08f8dbc7dac6501c028d9263480e3bf7a077c06922ae4e4ade759bcfc570ae2f53481f167c9f5def37409e57ae96aa157165a637fc'
  '48d44637370a47564d9f5d6281dae0595d3be1d0ad471de3dde2c82547ef3e47e4319c0da027241048a501fca3730a2e77a46525f192d26ca480db833fa03c2f'
)

package() {
  cd $srcdir
  install -Dm555 $pkgname-$pkgver $pkgdir/usr/bin/$pkgname
  install -Dm555 $pkgname.desktop $pkgdir/usr/share/applications/$pkgname.desktop
}
