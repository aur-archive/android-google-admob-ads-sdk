# Maintainer: Jakub Schmidtke <sjakub-at-gmail-dot-com>

pkgname=android-google-admob-ads-sdk
pkgver=4.3.1
pkgrel=1
pkgdesc='Google AdMob Ads SDK'
arch=('any')
url="https://developers.google.com/mobile-ads-sdk"
license=('custom')
depends=('android-sdk')
source=("https://dl-ssl.google.com/googleadmobadssdk/googleadmobadssdkandroid-${pkgver}.zip" "source.properties")
sha1sums=('e0fe9835b5c676e25e0bf215e8f44c1bc8ef172d' 'bfc44c21aa315d5bd082cbe61d82ad6bdc471620')

package() {
  mkdir -p "${pkgdir}/opt/android-sdk/extras/google/"
  mv "${srcdir}/GoogleAdMobAdsSdkAndroid-${pkgver}" "${pkgdir}/opt/android-sdk/extras/google/admob_ads_sdk"
  cp "${srcdir}/source.properties" "${pkgdir}/opt/android-sdk/extras/google/admob_ads_sdk/"

  chmod -R ugo+rX "${pkgdir}/opt"
}
