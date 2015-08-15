pkgname=gpskt-bin
pkgver=1.7
pkgrel=1

pkgdesc="Algorithms and frameworks supporting the development of processing and analysis applications in navigation and global positioning."
url="http://sourceforge.net/projects/gpstk"
license=('LGPL')

depends=()
makedepends=()
optdepends=()
provides=('gpstk')
conflicts=('gpstk')

arch=('i686')

if [[ $CARCH == i686 ]]; then
source=(http://sourceforge.net/projects/gpstk/files/gpstk/$pkgver/gpstk-$pkgver.linux.x386.tar.gz)
md5sums=('8eb58bb24f7309adf2204fe16449e865')
else
source=(http://sourceforge.net/projects/gpstk/files/gpstk/$pkgver/gpstk-$pkgver.linux.amd64.tar.gz)
md5sums=('23cc7cf61844cf67ed91107dde749578')
fi

build() {
cd $srcdir/gpstk
mkdir $pkgdir/usr

cp -r $srcdir/gpstk/bin $pkgdir/usr
cp -r $srcdir/gpstk/include $pkgdir/usr
cp -r $srcdir/gpstk/lib $pkgdir/usr

}
