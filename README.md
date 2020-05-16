```
cd /tmp
sudo $HOME/go/bin/distrobuilder build-lxd $HOME/Development/lxc-ci/images/ubuntu.yaml \
    -o image.architecture=amd64 \
    -o image.release=focal \
    -o image.variant=xfce \
    -o source.url="http://us.archive.ubuntu.com/ubuntu"
lxc image import lxd.tar.xz rootfs.squashfs --alias xubuntu
```
