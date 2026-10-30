NAME="make"
VERSION="4.4.1"
SOURCE="https://ftp.gnu.org/gnu/make/make-4.4.1.tar.gz"
SHA256="dd16fb1d67bfab79a72f5e8390735c49e3e8e70b4945a15ab1f81ddb78658fb3"

DEPENDS=()

BUILD() {
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
