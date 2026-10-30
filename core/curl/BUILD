NAME="curl"
VERSION="8.16.0"
SOURCE="https://curl.se/download/curl-8.16.0.tar.xz"
SHA256="40c8cddbcb6cc6251c03dea423a472a6cea4037be654ba5cf5dec6eb2d22ff1d"

DEPENDS=("openssl" "zlib")

BUILD() {
    ./configure \
        --prefix=/usr \
        --with-openssl

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
