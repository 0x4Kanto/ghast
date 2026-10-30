NAME="xz"
VERSION="5.8.1"
SOURCE="https://github.com/tukaani-project/xz/releases/download/v5.8.1/xz-5.8.1.tar.xz"
SHA256="0b54f79df85912504de0b14aec7971e3f964491af1812d83447005807513cd9e"

DEPENDS=()

BUILD() {
    ./configure \
        --prefix=/usr \
        --disable-static \
        --enable-shared

    make -j"$JOBS"
}

INSTALL() {
    make DESTDIR="$DESTDIR" install
}
