NAME="ncurses"
VERSION="6.5"

SOURCE="https://ftp.gnu.org/gnu/ncurses/ncurses-6.5.tar.gz"

DEPENDS=()

BUILD() {
    ./configure \
        --prefix=/usr \
        --with-shared \
        --without-debug \
        --enable-widec \
        --with-termlib

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
