NAME="zlib"
VERSION="1.3.1"
SOURCE="https://zlib.net/fossils/zlib-1.3.1.tar.gz"
SHA256="9a93b2b7dfdac77ceba5a558a580e74667dd6fede4585b91eefb60f03b72df23"

DEPENDS=()

BUILD() {
    ./configure \
        --prefix=/usr

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
