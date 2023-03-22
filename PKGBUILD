# Maintainer: StormOSDev <linuxstormos@gmail.com>
pkgname=xero-xfce-config
_destname1="/etc"
pkgver=Rolling
pkgrel=3
pkgdesc="Desktop Config for xeroce"
arch=('any')
url="https://github.com/bfitzgit23"
license=('GPL3')
makedepends=('git')
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${srcdir}/${pkgname}/push.sh
	rm ${srcdir}/${pkgname}/README.md
	rm ${srcdir}/${pkgname}/PKGBUILD
}
