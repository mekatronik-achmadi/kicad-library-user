pkgname=kicad-library-user
pkgver=0.1
pkgrel=1
pkgdesc="Unofficial additional KiCad libraries"
arch=('any')
url="https://github.com/mekatronik-achmadi/kicad-library-user"
license=('Custom')
depends=('kicad')
source=('git+https://github.com/mekatronik-achmadi/kicad-library-user.git')
md5sums=('SKIP')

package(){
	cd $srcdir/$pkgname/

	mkdir -p $pkgdir/usr/share/kicad/userlib/symbols/user
	cp symbols/* $pkgdir/usr/share/kicad/userlib/symbols/user/

	mkdir -p $pkgdir/usr/share/kicad/userlib/footprints/user
	cp footprints/* $pkgdir/usr/share/kicad/userlib/footprints/user/

	mkdir -p $pkgdir/usr/share/kicad/userlib/packages3d/user
}
