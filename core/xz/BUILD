NAME="xz"
VERSION="5.8.1"

SOURCE="https://github.com/tukaani-project/xz/releases/download/v5.8.1/xz-5.8.1.tar.xz"

DEPENDS=()

BUILD() {
    ./configure \
        --prefix=/usr \
        --disable-static \
        --enable-shared

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
