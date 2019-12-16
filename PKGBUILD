pkgname=kicad-library-user
pkgver=0.1
pkgrel=1
pkgdesc="Unofficial additional KiCad libraries"
arch=('any')
url="https://github.com/mekatronik-achmadi/kicad-library-user"
license=('Custom')
depends=('kicad')
source=('git+https://github.com/mekatronik-achmadi/kicad-library-user.git'
	'git+https://github.com/apeng2012/apeng-kicad.git')
md5sums=('SKIP' 'SKIP')

package(){
	mkdir -p $pkgdir/usr/share/kicad/userlib/{footprints,packages3d,symbols}

	cd $srcdir/$pkgname/
	cp symbols/* $pkgdir/usr/share/kicad/userlib/symbols/
	mkdir -p $pkgdir/usr/share/kicad/userlib/footprints/user
	cp footprints/* $pkgdir/usr/share/kicad/userlib/footprints/user/

	cd $srcdir/apeng-kicad/
	cp library/* $pkgdir/usr/share/kicad/userlib/symbols/
	cp -r footprints/* $pkgdir/usr/share/kicad/userlib/footprints/
	cp -r packages3d/* $pkgdir/usr/share/kicad/userlib/packages3d/
}
