# Maintainer: Kwimy
pkgname=kwimy-luks
pkgver=0.0.1
pkgrel=1
pkgdesc="Kwimy Plymouth LUKS theme"
arch=('any')
url="https://github.com/KwimyOS"
license=('custom')
source=()
sha256sums=()

prepare() {
  rm -rf "$srcdir/kwimy-luks"
  mkdir -p "$srcdir/kwimy-luks"

  # Copy all files from startdir to srcdir/kwimy-luks, including hidden ones,
  # but excluding pkg, src, and the PKGBUILD itself to avoid recursion.
  find "$startdir" -maxdepth 1 \
    -not -path "$startdir" \
    -not -name "src" \
    -not -name "pkg" \
    -not -name "PKGBUILD" \
    -not -name "*.pkg.tar.*" \
    -not -name ".SRCINFO" \
    -exec cp -r {} "$srcdir/kwimy-luks/" \;
}

package() {
  install -d "$pkgdir/usr/share/plymouth/themes/kwimy-luks"
  cp -a "$srcdir/kwimy-luks/." \
    "$pkgdir/usr/share/plymouth/themes/kwimy-luks/"
}
