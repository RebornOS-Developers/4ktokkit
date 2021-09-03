# Maintainer: Rafael <rafael@rebornos.org>
# v0.9.5.0130

pkgname=4ktokkit
pkgver=0.9.5
pkgrel=1
pkgdesc="Enjoy videos anywhere, anytime regardless of whether you are offline."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('5aeaeaf5d14fc3a6dde3ea25e6b45a7003c24fdc7d87526c6970e8fc0092735e51d000b4260f516a467d63a43f1a781c44eb1e53c3505e0b26a75daef1c99493')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

