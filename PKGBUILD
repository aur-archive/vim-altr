pkgname=vim-altr
pkgver=0.2.0
pkgrel=1
pkgdesc="Switch to the missing file without interaction"
arch=('any')
url="https://github.com/kana/vim-altr"
license=('MIT/X')
depends=('vim>=7.2')
groups=('vim-plugins')
install=vimdoc.install
source=($pkgname-$pkgver.tar.gz::"https://github.com/kana/vim-altr/archive/${pkgver}.tar.gz")
sha1sums=('265bb4138c7c78551f2838261b86bf865a86d909')

package() {
	cd "$srcdir/$pkgname-$pkgver"
	installpath="$pkgdir/usr/share/vim/vimfiles"
	install -Dm644 autoload/altr.vim $installpath/autoload/altr.vim
	install -Dm644 doc/altr.txt $installpath/doc/altr.txt
	install -Dm644 plugin/altr.vim $installpath/plugin/altr.vim
}
