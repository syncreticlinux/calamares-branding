# $Id$
# Maintainer: James Kittsmiller (AJSlye) <james@nulogicsystems.com>

pkgname=netrunner-calamares-branding
pkgver=$(date +%Y%m%d)
pkgrel=1
pkgdesc='Netrunner calamares branding'
arch=('any')
url="https://github.com/netrunner-rolling/netrunner-calamares-branding"
license=('GPL')
depends=('calamares')
makedepends=('git')
install=netrunner-calamares-branding.install
source=("git+$url.git")
sha256sums=('SKIP')

package() {
	install -d $pkgdir/usr/share/calamares/branding/netrunner
	install -d $pkgdir/usr/share/icons/hicolor/128x128/apps/
	cp ${srcdir}/${pkgbase}/netrunner/* $pkgdir/usr/share/calamares/branding/netrunner
	cp ${srcdir}/${pkgbase}/calamares-netrunner.png $pkgdir/usr/share/icons/hicolor/128x128/apps/calamares-netrunner.png
}
