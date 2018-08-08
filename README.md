openwrt-builder
========================

This is a docker container for building [OpenWRT](https://openwrt.org/)


To run a shell in the buildroot, execute the following command:
```sh
docker run --rm -it alljoynsville/openwrt-builder:18.06 bash
```
or
```sh
docker run --rm -it alljoynsville/openwrt-builder:15.05 bash
```

and then
```sh
cd /home/openwrt/openwrt
./scripts/feeds update -a
./scripts/feeds install -a

make defconfig
make
```
