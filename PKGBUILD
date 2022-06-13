# This is an example PKGBUILD file. Use this as a start to creating your own,
# and remove these comments. For more information, see 'man PKGBUILD'.
# NOTE: Please fill out the license field for your package! If it is unknown,
# then please put 'unknown'.

# Maintainer: Alfred Roos <alfred@stensatter.se>
pkgname=Calcer-git
pkgver=1
pkgrel=1
epoch=
pkgdesc="Calculator for i3"
arch=(x86_64)
url=""
license=('MIT')
groups=()
depends=()
makedepends=(git)
checkdepends=()
optdepends=()
provides=()
conflicts=()
replaces=()
backup=()
options=()
install=
changelog=
source=(git+$url)
noextract=()
md5sums=()
validpgpkeys=()

prepare() {
    git clone $url calcergit
    git clone https://github/spynetS/JCalc.git

}
package() {
    
    mv ./JCalc/out/artifacts/TerminalKalkylator_jar/TerminalKalkylator.jar /usr/bin/JCalc.jar
    mv ./calcergit/calcer /usr/bin/calcer

}
