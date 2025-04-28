# OpenStick Packages Feed

## Description

This is an OpenWrt package feed containing firmware and utils packages used in DongleWrt.

## Usage

To use these packages, add the following line to the feeds.conf
in the OpenWrt buildroot:

```
src-git openstick https://github.com/donglewrt/openstick.git
```

This feed should be included and enabled by default in the OpenWrt buildroot. To install all its package definitions,
run:

```
./scripts/feeds update openstick
./scripts/feeds install -a -p openstick
```

The openstick packages should now appear in menuconfig.

## License

OpenStick is licensed under GPLv2

## Credits

- [aa889788/openstick-feeds](https://github.com/aa889788/openstick-feeds)
- [HandsomeMod/HandsomeMod](https://github.com/HandsomeMod/HandsomeMod)
- [lkiuyu/openstick-feeds](https://github.com/lkiuyu/openstick-feeds)
