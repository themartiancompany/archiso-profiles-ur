# Maintainer: Pellegrino Prevete <pellegrinoprevete@gmail.com>

pkgname=archiso-profiles
pkgver=0.1
pkgrel=1
pkgdesc='Tools for creating Arch Linux live and install iso images with luks'
arch=('any')
license=('GPL3')
url="https://gitlab.archlinux.org/tallero/${pkgname}"
depends=('archiso-encryption')
makedepends=('git')
checkdepends=('shellcheck')
optdepends=()
source=("git+${url}")
sha256sums=('SKIP')

package() {
  local _profiles_dir="${pkgdir}/usr/share/archiso/configs"

  install -dm755 "${_profiles_dir}"
  cp -r "${srcdir}/${pkgname}/encrypted" "${_profiles_dir}"
}