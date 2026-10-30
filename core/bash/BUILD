NAME="bash"
VERSION="5.3"
SOURCE="https://ftp.gnu.org/gnu/bash/bash-5.3.tar.gz"

DEPENDS=("readline" "ncurses")

BUILD() {
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
