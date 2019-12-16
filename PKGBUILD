pkgname=kicad-library-user
pkgver=0.1
pkgrel=1
pkgdesc="Unofficial additional KiCad libraries"
arch=('any')
url="https://github.com/mekatronik-achmadi/kicad-library-user"
license=('Custom')
depends=('kicad')
source( 'git+https://github.com/mekatronik-achmadi/kicad-library-user.git'
	'git+https://github.com/apeng2012/apeng-kicad.git')
md5sums=('SKIP' 'SKIP')

pkgver() {
	cd "${srcdir}/toastpp"
	printf "%s" "$(git describe --tags | sed 's/\([^-]*-\)g/r\1/;s/-/./g;s/^rel\.//')"
}

package(){
	cd $srcdir/$pkgname

}
