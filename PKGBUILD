# Maintainer: buom <39004+buom@users.noreply.github.com>
pkgname=f5vpn
pkgver=0.2
pkgrel=1
epoch=
pkgdesc="SSL VPN application"
arch=('x86_64')
url="https://devcentral.f5.com/s/question/0D51T00006i7kIB/f5-ssl-vpn-on-unsupported-linux-distribution-arch-linux-manjaro-maybe-others"
license=('Commercial')
provides=("${pkgname}")
install=$pkgname.install
source=("https://f5vpn.geneseo.edu/public/download/linux_${pkgname}.x86_64.deb")
md5sums=('ed8e5772bc1a595ef5db70e82951d1d6')
depends=(icu openssl qt5-base)

package() {
	cd "${srcdir}"
	tar zvxf data.tar.gz
	cp -vr opt/ $pkgdir/
}

