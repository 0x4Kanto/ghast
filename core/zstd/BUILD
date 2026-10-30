NAME="zstd"
VERSION="1.5.7"
SOURCE="https://github.com/facebook/zstd/releases/download/v1.5.7/zstd-1.5.7.tar.gz"
SHA256="eb33e51f49a15e023950cd7825ca74a4a2b43db8354825ac24fc1b7ee09e6fa3"

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
