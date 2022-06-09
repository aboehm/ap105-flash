# Flash Tool for Aruba AP-105

Tool to exchange Aruba AP-105 boot loader with uboot for flashing OpenWRT.

## Usage

```
ap105-flash <SERIAL NUMBER>
```

The flash will be secured into files:

- `AP105-<SERIAL NUMBER>-dump0.rom`
- `AP105-<SERIAL NUMBER>-dump1.rom`

The `AP105-<SERIAL_NUMBER>-dump0.rom` will be patched with uboot binary `uboot.bin` and the file `AP105-<SERIAL NUMBER>-patch.rom` will be created.

After a confirmation the patched file will be flashed to the device.

## Sources

- [git repository for uboot loader @chunkey](https://github.com/chunkeey/u-boot-ap105/releases)
- [OpenWRT device page](https://openwrt.org/toh/aruba/ap-105)
