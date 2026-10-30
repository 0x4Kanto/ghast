NAME="readline"
VERSION="8.3"

SOURCE="https://ftp.gnu.org/gnu/readline/readline-8.3.tar.gz"

DEPENDS=("ncurses")

BUILD() {
    ./configure \
        --prefix=/usr \
        --with-curses \
        --enable-shared

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
