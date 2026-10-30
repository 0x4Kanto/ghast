NAME="openssl"
VERSION="3.5.4"

SOURCE="https://www.openssl.org/source/openssl-3.5.4.tar.gz"

DEPENDS=()

BUILD() {
    ./Configure \
        --prefix=/usr \
        --openssldir=/etc/ssl \
        --libdir=lib \
        shared

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install_sw
}
