
pkgname=calamares-branding
pkgver=$(date +%Y%m%d)
pkgrel=1
pkgdesc='Syncretic calamares branding'
arch=('any')
url="https://github.com/syncreticlinux/calamares-branding"
license=('GPL')
depends=('calamares')
makedepends=('git')
install=calamares-branding.install
source=("git+$url.git")
sha256sums=('SKIP')

package() {
	install -d $pkgdir/usr/share/calamares/branding/syncretic
	install -d $pkgdir/usr/share/icons/hicolor/128x128/apps/
	cp ${srcdir}/${pkgbase}/syncretic/* $pkgdir/usr/share/calamares/branding/syncretic
	#cp ${srcdir}/${pkgbase}/calamares-syncretic.png $pkgdir/usr/share/icons/hicolor/128x128/apps/calamares-syncretic.png
}
