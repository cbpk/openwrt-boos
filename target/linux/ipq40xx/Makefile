include $(TOPDIR)/rules.mk

ARCH:=arm
BOARD:=ipq40xx
BOARDNAME:=Qualcomm Atheros IPQ40XX
FEATURES:=squashfs fpu ramdisk nand
CPU_TYPE:=cortex-a7
CPU_SUBTYPE:=neon-vfpv4
SUBTARGETS:=generic

KERNEL_PATCHVER:=5.10

KERNELNAME:=zImage Image dtbs

include $(INCLUDE_DIR)/target.mk
DEFAULT_PACKAGES += \
	kmod-usb-dwc3-qcom \
	kmod-leds-gpio kmod-gpio-button-hotplug swconfig \
	kmod-ath10k-ct wpad-openssl uboot-envtools \
	kmod-usb3 kmod-usb-dwc3 ath10k-firmware-qca4019-ct \
	autocore-arm automount autosamba luci-app-eqos luci-app-cpufreq luci-app-zerotier \
	htop ethtool

$(eval $(call BuildTarget))
