https://github.com/paritytech/parity-ethereum

Download from source

Fresh ubuntu, so get curl:
sudo apt-get curl

Rustup:
curl https://sh.rustup.rs -sSf | sh

rustup --version

Verify the following:
gcc, g++, libudev-dev, pkg-config, file, make, and cmake

I was missing libudev-dev and cmake. Used apt-get for both of these
https://github.com/paritytech/parity-ethereum/issues/4546


Didn't need to download Perl: https://www.perl.org/get.html#unix_like
YASM needed to download: https://yasm.tortall.net/Download.html
^had to use sudo make install to get this

git checkout beta
cargo build --release --features final
./target/release/parity

Warp sync automatically starts:
https://wiki.parity.io/Getting-Synced
