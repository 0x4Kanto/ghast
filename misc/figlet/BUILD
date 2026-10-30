NAME="figlet"
VERSION="2.2.5"
SOURCE="https://fossies.org/linux/misc/old/figlet-2.2.5.tar.gz"
SHA256="bf88c40fd0f077dab2712f54f8d39ac952e4e9f2e1882f1195be9e5e4257417d"

DEPENDS=()

BUILD() {
    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" prefix=/usr install
}
