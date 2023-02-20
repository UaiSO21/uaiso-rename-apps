# Maintainer: Bruno Goncalves <bigbruno@gmail.com>

pkgname=uaiso-rename-apps
pkgver=$(date +%y.%m.%d)
pkgrel=$(date +%H%M)
arch=('any')
license=('GPL')
url="https://github.com/UaiSO21/uaiso-rename-apps"
pkgdesc="Rename apps"
conflicts=('bashrc-manjaro' 'biglinux-apps-rename')
provides=('bashrc')
source=("git+https://github.com/UaiSO21/uaiso-rename-apps.git")
md5sums=(SKIP)

package() {
    # Verify default folder
    if [ -d "${srcdir}/${pkgname}" ]; then
        InternalDir="${srcdir}/${pkgname}"
    else
        InternalDir="${srcdir}/${pkgname}"
    fi


    # Copy files
    if [ -d "${InternalDir}/usr" ]; then
        cp -r "${InternalDir}/usr" "${pkgdir}/"
    fi

    if [ -d "${InternalDir}/etc" ]; then
        cp -r "${InternalDir}/etc" "${pkgdir}/"
    fi

    if [ -d "${InternalDir}/opt" ]; then
        cp -r "${InternalDir}/opt" "${pkgdir}/"
    fi
}
