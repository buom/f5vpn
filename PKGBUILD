# Maintainer: buom <39004+buom@users.noreply.github.com>
pkgname=f5vpn-bin
_pkgname=f5vpn
pkgver=7182.2019.0923.1
pkgrel=2
epoch=
pkgdesc="This software can establish SSL VPN network access connection with F5 BIG-IP APM"
arch=('x86_64')
url="https://devcentral.f5.com/s/question/0D51T00006i7kIB/f5-ssl-vpn-on-unsupported-linux-distribution-arch-linux-manjaro-maybe-others"
license=('Commercial')
provides=("${pkgname}")
install=$pkgname.install
conflicts=('f5vpn')
source=("https://f5vpn.geneseo.edu/public/download/linux_${_pkgname}.x86_64.deb")
md5sums=('ed8e5772bc1a595ef5db70e82951d1d6')
depends=(icu openssl qt5-base)

package() {
	cd "${srcdir}"
	tar zvxf data.tar.gz
	cp -vr opt/ $pkgdir/
}

