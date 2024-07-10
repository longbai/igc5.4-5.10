# igc5.4-5.10
intel i225/226 driver backport from 5.10 to 5.4, add 226 hardware id from 6.9

from https://github.com/torvalds/linux/tree/v5.10/drivers/net/ethernet/intel/igc

compile with kernel-dev 5.4

# install gcc

```
yum --enablerepo=extras install centos-release-scl-rh
yum install devtoolset-9-gcc
scl enable devtoolset-9 bash
# 永久
# source /opt/rh/devtoolset-9/enable
```
# compile 
```
make -C /usr/src/kernels/5.4.199-200.cjktty.el7.x86_64/ M=`pwd` modules
```
