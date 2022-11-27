#install qemu

* You may need to install ninja

* tar -xf qemu-7.1.0.tar.gz
* cd qemu-7.1.0
* ./configure --prefix=/opt/qemu7 
* make && make install

# build kernel image for arm64

* make ARCH=arm64 CROSS_COMPILE=aarch64-none-linux-gnu- defconfig/menuconfig(for special settings)
* make ARCH=arm64 CROSS_COMPILE=aarch64-none-linux-gnu- Image -j8


