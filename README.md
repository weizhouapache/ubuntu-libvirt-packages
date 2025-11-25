# Libvirt packages on Ubuntu

It looks like the libvirt 10.0.0 causes CPU increase and delays VM actions after a few days.
Refer to https://github.com/apache/cloudstack/issues/11141

Installing newer libvirt might fix the issue

## Download ZIP file

```
wget https://github.com/weizhouapache/ubuntu-libvirt-packages/archive/refs/heads/main.zip
```

## Uncompress

```
unzip main.zip
cd ubuntu-libvirt-packages-main/
```

## Install new packages

```
cd libvirt-10.6.0-1ubuntu3.3
apt install ./libvirt*.deb
```

## Verify

```
virsh version
```
