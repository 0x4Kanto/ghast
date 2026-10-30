NAME="readline"
VERSION="8.3"
SOURCE="https://ftp.gnu.org/gnu/readline/readline-8.3.tar.gz"
SHA256="fe5383204467828cd495ee8d1d3c037a7eba1389c22bc6a041f627976f9061cc"

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
