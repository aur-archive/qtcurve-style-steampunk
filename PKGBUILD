# Maintainier Miguel Aguilar <zodiac_es@yahoo.es> 

pkgname=qtcurve-style-steampunk
pkgver=5.0
pkgrel=4
pkgdesc="SteampunK QtCurve light theme. This item is a part of Steam-Powered Linux KDE theme set."
arch=('any')
url="http://kde-look.org/content/show.php?content=142139"
license=('CCPL-by-sa')
groups=(steam-powered-linux)
depends=('qtcurve-kde4')
optdepends=('qtcurve-gtk2')
source=(http://sites.google.com/site/binaryinspiration/download/SteampunK.qtcurve)
md5sums=('f914f60aa79f79b272b23412bcbf0896')

package() {
   install -d $pkgdir/usr/share/apps/QtCurve
   cp -rf Steampun* $pkgdir/usr/share/apps/QtCurve/
   cat $srcdir/SteampunK.qtcurve | \
             sed -r 's/SteampunK-bgnd.jpg/\/usr\/share\/apps\/QtCurve\/SteampunK-bgnd.jpg/' > \
             $pkgdir/usr/share/apps/QtCurve/SteampunK.qtcurve

   chmod 644 $pkgdir/usr/share/apps/QtCurve/*
}
