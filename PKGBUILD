pkgname=codepad-git
_gitname=codepad
pkgver=0.2.3
pkgrel=1
pkgdesc="A codepad.org pastebin tool with options for syntax highlighting"
arch=(i686 x86_64)
license=('GPLv2')
depends=('python')
url=("https://github.com/kevr/$_gitname")
md5sums=("SKIP")
install=${pkgname}.install

package() {

  if [[ ! -d "$srcdir/$_gitname" ]]; then
    git clone "$url"
  fi

  cd "$srcdir/$_gitname"

  ./setup.py install --prefix="$pkgdir/usr/local" --yes &> /dev/null

}

