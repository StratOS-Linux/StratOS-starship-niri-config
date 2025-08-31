# Maintainer: @magitian <magitian@duck.com>
pkgname=stratos-starship-config
pkgver=1.0
pkgrel=3
pkgdesc="Starship configuration for StratOS Niri spin"
arch=('any')
license=('GPL3')
depends=(
    'starship'
)
source=()
install=stratos-starship-config.install

prepare() {
    cp -r "$startdir/.config/" "$srcdir/"
}

package() {
    install -d "$pkgdir/etc/skel/.config"
    cp -r "$srcdir/.config/starship/" "$pkgdir/etc/skel/.config/"
    cp "$srcdir/.config/starship/onedark/starship.toml" "$pkgdir/etc/skel/.config/starship.toml"
}
