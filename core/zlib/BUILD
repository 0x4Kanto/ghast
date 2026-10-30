NAME="zlib"
VERSION="1.3.1"

SOURCE="https://zlib.net/fossils/zlib-1.3.1.tar.gz"

DEPENDS=()

BUILD() {
    ./configure \
        --prefix=/usr

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
