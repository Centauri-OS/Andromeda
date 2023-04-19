# **Introducing**
The name of this custom kernel is 'Andromeda'. It is a fusion of two existing kernel variants - Hardened and TKPG-PDS. The 'Hardened' component refers to the kernel being hardened with additional security features, while 'TKPG-PDS' stands for 'Team Kirkwood's Gentoo Patches with PDS scheduler'.

The PDS scheduler in the TKPG-PDS variant is designed to improve system responsiveness and reduce latency, making the kernel ideal for multitasking and handling heavy workloads. The Gentoo patches used in the TKPG-PDS variant provide additional optimizations and features, such as CPU scheduler tweaks, network congestion control improvements, and filesystem performance enhancements.

Together with the added security features of the Hardened variant, the Andromed kernel is a powerful and robust system that delivers both speed and security. Whether you are a power user or a security-conscious individual, the Andromed kernel is designed to meet your needs and provide a reliable and efficient computing experience.
# **Pre-requisites**
```
gcc (compiler needed to make it work)
git (to copy the repository)
Free Space: 7GB
```
**To install the GCC you can follow this tutorial:**
```
tar -xzf gcc-4.6.2.tar.gz
cd gcc-4.6.2
./contrib/download_prerequisites
cd ..
mkdir objdir
cd objdir
$PWD/../gcc-4.6.2/configure --prefix=$HOME/GCC-4.6.2 --enable-languages=c,c++,fortran,go
make
make install
```
**And for git that, if you use doas or any alternative means of authentication sudo, remember to replace sudo with it:**
```
tar -zxf git-2.8.0.tar.gz
cd git-2.8.0
make configure
./configure --prefix=/usr
make all doc info
sudo make install install-doc install-html install-info
```
**To see if you have the necessary space:**
```
df -h /
```
