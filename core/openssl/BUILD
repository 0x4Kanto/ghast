NAME="openssl"
VERSION="3.5.4"
SOURCE="https://www.openssl.org/source/openssl-3.5.4.tar.gz"
SHA256="967311f84955316969bdb1d8d4b983718ef42338639c621ec4c34fddef355e99"

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
