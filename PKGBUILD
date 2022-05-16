pkgname=ddos-calamares-config
_destname1="/etc"
pkgver=1.0
pkgrel=01
groups=("ddos_installer")
pkgdesc="calamares config for ddos"
arch=('any')
license=('GPL3')
makedepends=('git')
depends=()
conflicts=('manjaro-system')

xserver="https://github.com"
xusername="ddosx"
xreponame="ddos-calamares-config"

url="${xserver}/${xusername}/${xreponame}.git"
provides=("${pkgname}")
options=(!strip !emptydirs)
source=("git+${url}")
sha256sums=('SKIP')

package() {
	install -dm755 ${pkgdir}${_destname1}
	mkdir -p ${pkgdir}${_destname1}/calamares
	cp -r ${srcdir}/${xreponame}${_destname1}/calamares/* ${pkgdir}${_destname1}/calamares/
}
