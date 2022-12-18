# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Your Name <keyaedisa>
pkgname="vnanorc"
pkgver=1.0
pkgrel=0
epoch=
pkgdesc="Keyaedisa's nano config made for Valen and XeroLinux (and whoever else :))"
arch=('x86_64' 'i686')
url="https://github.com/keyaedisa/vnanorc"
#license=('')
#groups=()
depends=("git"
		"nano"
		"nano-syntax-highlighting"
		)
makedepends=('git')
#checkdepends=()
#optdepends=()
provides=('vnanorc')
#conflicts=('')
#replaces=('')
#backup=()
#options=()
install=vnanorc.install
#changelog=
source=("gclone"::"git+https://github.com/keyaedisa/vnanorc.git")
#noextract=()
#md5sums=()
sha256sums=('SKIP')

package() {
	mv "${srcdir}/gclone/vnanorc" "${pkgdir}/etc/nanorc"
	rm -r "../gclone"
	rm -r "${srcdir}"
}


