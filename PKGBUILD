# Maintainer: Warren Guy <aur@warreng.uy>

pkgname=ttf-ioskeley-mono-term-nerd
pkgver=2.1.0
pkgrel=1
pkgdesc='Ioskeley Mono Term with single-width Nerd Font icons for terminals'
arch=('any')
url='https://github.com/ahatem/IoskeleyMono'
license=('OFL-1.1')
conflicts=('ttf-ioskeley-mono-nerd' 'ttf-ioskeley-mono-nerd-unhinted')
options=('!strip')
source=(
    "IoskeleyMono-Term-NerdFont-${pkgver}.zip::${url}/releases/download/v${pkgver}/IoskeleyMono-Term-NerdFont.zip"
    "OFL-1.1.txt::${url}/raw/v${pkgver}/LICENSE"
)
sha256sums=(
    '2eb905184e40602f6711d84c28448a0056a77de96881bbdee55b9595d40f2265'
    '1084285bd2bddf706d566e11a92fcbae2706da4a8eafac49ed34c871d01fb7fe'
)

package() {
    install -Dm644 -t "${pkgdir}/usr/share/fonts/TTF" \
        Normal/*.ttf \
        SemiCondensed/*.ttf
    install -Dm644 OFL-1.1.txt "${pkgdir}/usr/share/licenses/${pkgname}/LICENSE"
}
