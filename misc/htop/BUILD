NAME="htop"
VERSION="3.4.1"
SOURCE="https://github.com/htop-dev/htop/archive/refs/tags/3.4.1.tar.gz"
SHA256="af9ec878f831b7c27d33e775c668ec79d569aa781861c995a0fbadc1bdb666cf"

DEPENDS=("ncurses")

BUILD() {
    ./autogen.sh
    ./configure --prefix=/usr
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
