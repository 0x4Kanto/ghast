NAME="zstd"
VERSION="1.5.7"

SOURCE="https://github.com/facebook/zstd/releases/download/v1.5.7/zstd-1.5.7.tar.gz"

DEPENDS=()

BUILD() {
    make -j"$JOBS" \
        PREFIX=/usr \
        LIBDIR=/usr/lib \
        BUILD_SHARED=yes \
        BUILD_STATIC=no
}

INSTALL() {
    make PREFIX=/usr \
        LIBDIR=/usr/lib \
        DESTDIR="$DESTDIR" \
        install
}
