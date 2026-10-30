NAME="tar"
VERSION="1.35"
SOURCE="https://ftp.gnu.org/gnu/tar/tar-1.35.tar.xz"
SHA256="4d62ff37342ec7aed748535323930c7cf94acf71c3591882b26a7ea50f3edc16"

DEPENDS=("xz" "zstd")

BUILD() {
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
