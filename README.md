/android/lineage/device/bananapi/m5/BoardConfig.mk

```

## Kernel modules
TARGET_KERNEL_EXT_MODULES := \
    rtk_btusb:kbuild \
    rtl8822cs/rtl88x2CS:kbuild \
+    8821cu/rtl8821CU:kbuild

```

~/android/lineage/device/bananapi/m5/init-files$

```
on boot
    insmod /vendor/lib/modules/rtk_btusb.ko
    insmod /vendor/lib/modules/8822cs.ko rtw_country_code=US ifname=wlan0 if2name=p2p0
+    insmod /vendor/lib/modules/8821cu.ko rtw_country_code=US ifname=wlan0 if2name=p2p0
```
