# Reference the [offical doc](https://download.libsodium.org/doc/installation).

Download a [tarball of libsodium](https://download.libsodium.org/libsodium/releases), preferably the latest `stable` version, then follow the ritual:

```
./configure
make && make check
sudo make install
```

## Q1: libsodium not found
Enter the following command and try again：

```
echo /usr/local/lib > /etc/ld.so.conf.d/usr_local_lib.conf
ldconfig
```
