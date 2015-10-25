pkgname=python-yad
pkgver=0.9.5
pkgrel=1
pkgdesc="Interface to yad for python. Inspired by the PyZenity Project"
arch=('x86_64')
url="https://gitlab.com/dvenkatsagar/$pkgname"
license=('GPL3+')
depends=('python3' 'yad')
makedepends=('git' 'python3-setuptools')
source=("https://pypi.python.org/packages/source/y/yad/yad-0.9.5.tar.gz#md5=0bee3601c25e455d20b2586cd2892b60")
sha512sums=('e8d29644b7c3aaba4673cf53957293a5cf2baac56fdc8af5882c4fb51316114acd6ee1a3999757b7ad3aaddb87c6b9b3a96b3eb386567e51e74a5877fc9a6937')

build() {
    cd "${srcdir}/yad-0.9.5"
    python3 setup.py build
}

package() {
    cd "${srcdir}/yad-0.9.5"
    python3 setup.py install --root="$pkgdir/" --optimize=1
}
