#!/bin/bash

# Disable various shellcheck rules that produce false positives in this file.
# Repository rules should be added to the .shellcheckrc file located in the
# repository root directory, see https://github.com/koalaman/shellcheck/wiki
# and https://archiv8.github.io for further information.
# shellcheck disable=SC2034,SC2154
# ToDo: Add files: User documentation
# ToDo: Add files: Tooling
# FixMe: Namcap warnings and errors

# Maintainer: Ross Clark <archiv8@artisteducator.com>
# Contributor: Ross Clark <archiv8@artisteducator.com>


pkgname=findbrokenpkgs
pkgver=1.1
pkgrel=2
pkgdesc="Broken package identifier for Arch Linux, based on Gentoo's revdep-rebuild"
arch=("any")
url="http://bbs.archlinux.org/viewtopic.php?id=13882"
license=("GPL")
depends=(
  "binutils"
  "pacman"
)
source=(
  "$pkgname-$pkgver.sh"
)
sha512sums=(
  "88f42116c41834c5f94d29a6010db3ebe4f151c91402558164356953e6059a44eba7aa6af6b8c4a9b4035f11f757574d546a618a26346360db0f0af4060af0fd"
)

package() {
  install -Dm755 $pkgname-$pkgver.sh "${pkgdir}"/usr/bin/$pkgname
}
