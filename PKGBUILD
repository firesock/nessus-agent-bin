pkgname="nessus-agent-bin"
pkgver="10.0.0"
pkgrel=5
pkgdesc="Agent binaries"
arch=("x86_64")
url="https://www.tenable.com/products/nessus/nessus-agents"
license=("custom")
depends=("glibc" "gcc-libs")
install="nessus-agent-bin.install"
source=("local://NessusAgent-$pkgver-fc20.x86_64.rpm")
sha256sums=("fd2c6bea63d1ff9b9840196de62ebf0a21c3d48942066a398bc3ba98ed512e81")

package() {
	cp --no-dereference --preserve=mode,links,timestamps --recursive opt usr "${pkgdir}"
}
