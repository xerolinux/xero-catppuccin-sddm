# Maintainer: DarkXero <info@techxero.com>
pkgname=xero-catppuccin-sddm
_destname1="/"
pkgver=0.1
pkgrel=2
pkgdesc="SDDM Theme"
arch=('any')
url="https://github.com/XeroLinux"
license=('GPL3')
makedepends=('git')
depends=()
conflicts=()
provides=("${pkgname}")
options=(!strip !emptydirs)
source=(${pkgname}::"git+${url}/${pkgname}")
sha256sums=('SKIP')
package() {
	install -dm755 ${pkgdir}${_destname1}
	cp -r ${srcdir}/${pkgname}${_destname1}/* ${pkgdir}${_destname1}
	rm ${pkgdir}${_destname1}/creds.sh
	rm ${pkgdir}${_destname1}/push.sh
	rm ${pkgdir}${_destname1}/PKGBUILD
	rm ${pkgdir}${_destname1}/LICENSE
}
