NAME="grep"
VERSION="3.12"
SOURCE="https://ftp.gnu.org/gnu/grep/grep-3.12.tar.xz"
SHA256="0d5cd86965f869a26cf64f4b71be7b96f90a3ba8b3d74e27e8e9d9d5550f31ba"

DEPENDS=()

BUILD() {
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
