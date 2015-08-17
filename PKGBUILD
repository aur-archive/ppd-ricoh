# Maintainer: Kelly Price <kellyjosephprice@gmail.com>
pkgname=ppd-ricoh
pkgver=4
pkgrel=1
pkgdesc="PPD files for Ricoh's PostScript printers, supplied by Ricoh"
arch=('i686' 'x86_64')
url="http://www.openprinting.org/driver/Postscript-Ricoh"
license=('MIT')
depends=('cups' 'foomatic-filters')
install=ricoh.install
source=('Postscript-Ricoh.ppd::http://www.openprinting.org/ppd-o-matic.php?driver=Postscript-Ricoh&printer=Ricoh-Aficio_SP_5210SF&show=0')
md5sums=('79eb614f0070d766dcc88efbc9102140')

build() {
  cd "$srcdir"
  install -d $pkgdir/usr/share/cups/model/Ricoh
  install Postscript-Ricoh.ppd $pkgdir/usr/share/cups/model/Ricoh
}

