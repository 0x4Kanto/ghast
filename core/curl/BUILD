NAME="curl"
VERSION="8.16.0"

SOURCE="https://curl.se/download/curl-8.16.0.tar.xz"

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
