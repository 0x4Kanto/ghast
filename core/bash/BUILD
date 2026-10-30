NAME="bash"
VERSION="5.3"
SOURCE="https://ftp.gnu.org/gnu/bash/bash-5.3.tar.gz"
SHA256="0d5cd86965f869a26cf64f4b71be7b96f90a3ba8b3d74e27e8e9d9d5550f31ba"

DEPENDS=("readline" "ncurses")

BUILD() {
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
