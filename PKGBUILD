# Maintainer: Rafael <rafael@rebornos.org>
# v	0.9.6.0140

pkgname=4ktokkit
pkgver=0.9.6
pkgrel=1
pkgdesc="Download all videos from TikTok hashtags and users in one click."
arch=('any')
url="https://dl.4kdownload.com/app"
license=('Custom')
makedepends=('make')
provides=(${pkgname})
conflicts=(${pkgname})
source=(${url}/${pkgname}_${pkgver}-${pkgrel}_amd64.deb)
sha512sums=('506545c4420bdf25f331548a4c2bac66aaa2904824698be620731ae7563a96a0ea5b9ff1557c248c6777c2ce95149c8e2b91cd38ae03604d95ee5abe50108844')

package() {
           mkdir -p ${pkgdir}/usr/bin
           tar -xvf ${srcdir}/data.tar.xz
           cp -r ${srcdir}/usr/* ${pkgdir}/usr/
           cp ${pkgdir}/usr/lib/${pkgname}/${pkgname}.sh ${pkgdir}/usr/bin/${pkgname}
}

