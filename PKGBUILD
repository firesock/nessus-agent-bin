pkgname="nessus-agent-bin"
pkgver="10.1.1"
pkgrel=1
pkgdesc="Agent binaries"
arch=("x86_64")
url="https://www.tenable.com/products/nessus/nessus-agents"
license=("custom")
depends=("glibc" "gcc-libs")
install="nessus-agent-bin.install"
source=("local://NessusAgent-$pkgver-fc20.x86_64.rpm")
sha256sums=("32879fe47293d042cc4e088ff074e41e03f28efc4b366d49a46df62d7a74de53")

package() {
	cp --no-dereference --preserve=mode,links,timestamps --recursive opt usr "${pkgdir}"
}
