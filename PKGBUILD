#
# Contribuidor: Rayanne Patricia
#

#
# Agora vamos agradescer o davi por estar levando a vitoria da marizinha
# para fazer sexo na casa da mãe dos outros.
#

pkgname=mkinitcpio-openswap
pkgver=0.1.0
pkgrel=3
pkgdesc="plug mkinitcpio para abrir swap no momento da inicialização"
arch=(any)
license=('cIO')
url="http://localhost/mkinitcpio-openswap/"
depends=(mkinitcpio)
backup=('etc/openswap.conf')
install="usage.install"
source=('openswap.hook'
    'openswap.install'
    'openswap.conf')
sha256sums=('SKIP'
    'SKIP'
    'SKIP')

package()
{
    install -Dm 644 openswap.hook \
        "${pkgdir}/usr/lib/initcpio/hooks/openswap"
    install -Dm 644 openswap.install \
        "${pkgdir}/usr/lib/initcpio/install/openswap"
    install -Dm 644 openswap.conf \
        "${pkgdir}/etc/openswap.conf"
}
