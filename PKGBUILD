pkgname=rp64-pwmconfig
pkgver=1.0
pkgrel=1
pkgdesc="RockPro64 PWM config"
arch=('any')
url="https://gitlab.com/nuumio-manjaro/rp64-pwmconfig"
license=('MIT')
depends=('bash>=5.0.0' 'inotify-tools>=3.20.0' 'systemd>=245.0')

source=('rp64-pwmconfig'
        'rp64-pwmconfig.conf'
        'rp64-pwmconfig.service')

sha256sums=('SKIP'
            'SKIP'
            'SKIP')

install=${pkgname}.install

package() {
  install -D "${srcdir}/rp64-pwmconfig" "${pkgdir}/usr/bin/rp64-pwmconfig"
  install -Dm644 "${srcdir}/rp64-pwmconfig.conf" "${pkgdir}/etc/rp64-pwmconfig.conf"
  install -Dm644 "${srcdir}/rp64-pwmconfig.service" "${pkgdir}/usr/lib/systemd/system/rp64-pwmconfig.service"
}
