pkgname=otf-gandhi-sans
pkgdesc="Gandhi Sans font family by Cristóbal Henestrosa and Raúl Plancarte for Librería Gandhi (OpenType)"
url='http://www.tipografiagandhi.com/'
license=('custom')
pkgver=1.001
pkgrel=1
arch=('any')
install=$pkgname.install

source=('gandhi-sans.zip::https://www.fontsquirrel.com/fonts/download/gandhi-sans')
sha256sums=('SKIP')

package() {
  install -d "${pkgdir}/usr/share/fonts/${pkgname}"
  cp -dpr --no-preserve=all "${srcdir}/"*.otf "${pkgdir}/usr/share/fonts/${pkgname}"
  install -D -m644 "${srcdir}/Librerias Gandhi S.A. de C.V. Font License.txt" "${pkgdir}/usr/share/licenses/${pkgname}/Librerias Gandhi S.A. de C.V. Font License.txt"
}
