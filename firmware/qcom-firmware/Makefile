#
# Copyright (C) 2020-2022 HandsomeMod Project
#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=qcom-firmware
PKG_VERSION:=1034.2.2
PKG_RELEASE:=2

PKG_SOURCE_PROTO:=git
PKG_SOURCE_URL:=https://github.com/donglewrt/qcom-firmwares.git
PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.xz
PKG_SOURCE_VERSION:=e5e7752f2bc3d545a142a0ba8dc9a4f29128412a
PKG_MIRROR_HASH:=7daefa9329c8a8f0b7ed581fc524cae004ed2a425038b844532bbeb45d1bb277

include $(INCLUDE_DIR)/package.mk

define Package/qcom-firmware-default
  SECTION:=firmware
  CATEGORY:=Firmware
endef

define Build/Compile
	mkdir -p $(PKG_BUILD_DIR)/dragonboard
	mcopy -i $(PKG_BUILD_DIR)/dragonboard-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/dragonboard
	mkdir -p $(PKG_BUILD_DIR)/openstick-ufi001b
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001b-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001b
	mkdir -p $(PKG_BUILD_DIR)/openstick-ufi001c
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi001c-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi001c
	mkdir -p $(PKG_BUILD_DIR)/openstick-ufi003
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi003-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi003
	mkdir -p $(PKG_BUILD_DIR)/openstick-ufi103s
	mcopy -i $(PKG_BUILD_DIR)/openstick-ufi103s-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-ufi103s
	mkdir -p $(PKG_BUILD_DIR)/openstick-sp970
	mcopy -i $(PKG_BUILD_DIR)/openstick-sp970-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-sp970
	mkdir -p $(PKG_BUILD_DIR)/openstick-uz801
	mcopy -i $(PKG_BUILD_DIR)/openstick-uz801-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-uz801
	mkdir -p $(PKG_BUILD_DIR)/openstick-qrzl903
	mcopy -i $(PKG_BUILD_DIR)/openstick-qrzl903-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-qrzl903
	mkdir -p $(PKG_BUILD_DIR)/openstick-w001
	mcopy -i $(PKG_BUILD_DIR)/openstick-w001-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-w001
	mkdir -p $(PKG_BUILD_DIR)/openstick-mf32
	mcopy -i $(PKG_BUILD_DIR)/openstick-mf32-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-mf32
	mkdir -p $(PKG_BUILD_DIR)/openstick-mf601
	mcopy -i $(PKG_BUILD_DIR)/openstick-mf601-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-mf601
	mkdir -p $(PKG_BUILD_DIR)/openstick-mfx32
	mcopy -i $(PKG_BUILD_DIR)/openstick-mfx32-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-mfx32
	mkdir -p $(PKG_BUILD_DIR)/openstick-wf2
	mcopy -i $(PKG_BUILD_DIR)/openstick-wf2-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/openstick-wf2
	mkdir -p $(PKG_BUILD_DIR)/wt88047
	mcopy -i $(PKG_BUILD_DIR)/wt88047-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt88047
	mkdir -p $(PKG_BUILD_DIR)/wt86047
	mcopy -i $(PKG_BUILD_DIR)/wt86047-modem.bin -p -m -n -v \
		::image/mba.mbn ::image/modem.* ::image/wcnss.* $(PKG_BUILD_DIR)/wt86047	
endef

define Package/qcom-apq8016-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI & Bluetooth firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick UFI001B
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick UFI001C
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick UFI003
endef

define Package/qcom-msm8916-openstick-ufi103s-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick UFI103S
endef

define Package/qcom-msm8916-openstick-sp970-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick SP970
endef

define Package/qcom-msm8916-openstick-uz801-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick UZ801
endef

define Package/qcom-msm8916-openstick-qrzl903-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick QRZL903
endef

define Package/qcom-msm8916-openstick-w001-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick W001
endef

define Package/qcom-msm8916-openstick-mf32-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick MF32
endef

define Package/qcom-msm8916-openstick-mf601-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick MF601
endef

define Package/qcom-msm8916-openstick-mfx32-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick MFX32
endef

define Package/qcom-msm8916-openstick-wf2-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Openstick WF2
endef

define Package/qcom-msm8916-wt8x047-wcnss
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI & Bluetooth firmware for Redmi 2
endef

define Package/qcom-apq8016-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 WIFI nv data
endef

define Package/qcom-msm8916-wt88047-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Wingtech Wt88047
endef

define Package/qcom-msm8916-openstick-ufi001b-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick UFI001B
endef

define Package/qcom-msm8916-openstick-ufi001c-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick UFI001C
endef

define Package/qcom-msm8916-openstick-ufi003-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick UFI003
endef

define Package/qcom-msm8916-openstick-ufi103s-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick UFI103S
endef

define Package/qcom-msm8916-openstick-sp970-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick SP970
endef

define Package/qcom-msm8916-openstick-uz801-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick UZ801
endef

define Package/qcom-msm8916-openstick-qrzl903-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick QRZL903
endef

define Package/qcom-msm8916-openstick-w001-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick W001
endef

define Package/qcom-msm8916-openstick-mf32-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick MF32
endef

define Package/qcom-msm8916-openstick-mf601-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick MF601
endef

define Package/qcom-msm8916-openstick-mfx32-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick MFX32
endef

define Package/qcom-msm8916-openstick-wf2-nv
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 WIFI nv data for Openstick WF2
endef

define Package/qcom-apq8016-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm apq8016 modem firmware
endef

define Package/qcom-msm8916-wt88047-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt88047
endef

define Package/qcom-msm8916-wt86047-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for wingtech wt86047
endef

define Package/qcom-msm8916-openstick-ufi001b-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick UFI001B
endef

define Package/qcom-msm8916-openstick-ufi001c-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick UFI001C
endef

define Package/qcom-msm8916-openstick-ufi003-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick UFI003
endef

define Package/qcom-msm8916-openstick-ufi103s-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick UFI103S
endef

define Package/qcom-msm8916-openstick-sp970-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick SP970
endef

define Package/qcom-msm8916-openstick-uz801-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick UZ801
endef

define Package/qcom-msm8916-openstick-qrzl903-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick QRZL903
endef

define Package/qcom-msm8916-openstick-w001-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick W001
endef

define Package/qcom-msm8916-openstick-mf32-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick MF32
endef

define Package/qcom-msm8916-openstick-mf601-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick MF601
endef

define Package/qcom-msm8916-openstick-mfx32-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick MFX32
endef

define Package/qcom-msm8916-openstick-wf2-modem
  $(Package/qcom-firmware-default)
  TITLE:=Qualcomm msm8916 modem firmware for Openstick WF2
endef

define Package/qcom-apq8016-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001c-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi003-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi103s-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-sp970-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-uz801-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-qrzl903-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-qrzl903/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-w001-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-w001/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mf32-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf32/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mf601-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf601/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mfx32-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mfx32/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-wf2-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-wf2/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-wt8x047-wcnss/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/wcnss.* \
		$(1)/lib/firmware
endef

define Package/qcom-apq8016-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-wt88047-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt8x047-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-ufi001b-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-ufi001c-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-ufi003-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-ufi103s-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-sp970-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-uz801-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-qrzl903-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-qrzl903-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-w001-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-w001-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-mf32-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf32-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-mf601-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf601-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-mfx32-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mfx32-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-msm8916-openstick-wf2-nv/install
	$(INSTALL_DIR) $(1)/lib/firmware/wlan/prima
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-wf2-nv.bin \
		$(1)/lib/firmware/wlan/prima/WCNSS_qcom_wlan_nv.bin
endef

define Package/qcom-apq8016-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/dragonboard/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-wt88047-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt88047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-wt86047-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/wt86047/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001b-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001b/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi001c-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi001c/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi003-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi003/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-ufi103s-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-ufi103s/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-sp970-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-sp970/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-uz801-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-uz801/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-qrzl903-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-qrzl903/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-qrzl903/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-w001-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-w001/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-w001/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mf32-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf32/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf32/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mf601-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf601/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mf601/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-mfx32-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mfx32/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-mfx32/modem.* \
		$(1)/lib/firmware
endef

define Package/qcom-msm8916-openstick-wf2-modem/install
	$(INSTALL_DIR) $(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-wf2/mba.mbn \
		$(1)/lib/firmware
	$(INSTALL_DATA) \
		$(PKG_BUILD_DIR)/openstick-wf2/modem.* \
		$(1)/lib/firmware
endef

$(eval $(call BuildPackage,qcom-apq8016-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-wt8x047-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001b-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001c-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi003-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi103s-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-sp970-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-qrzl903-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-w001-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf32-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf601-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mfx32-wcnss))
$(eval $(call BuildPackage,qcom-msm8916-openstick-wf2-wcnss))

$(eval $(call BuildPackage,qcom-apq8016-nv))
$(eval $(call BuildPackage,qcom-msm8916-wt88047-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001b-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001c-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi003-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi103s-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-sp970-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-qrzl903-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-w001-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf32-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf601-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mfx32-nv))
$(eval $(call BuildPackage,qcom-msm8916-openstick-wf2-nv))

$(eval $(call BuildPackage,qcom-apq8016-modem))
$(eval $(call BuildPackage,qcom-msm8916-wt88047-modem))
$(eval $(call BuildPackage,qcom-msm8916-wt86047-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001b-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi001c-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi003-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-ufi103s-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-sp970-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-uz801-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-qrzl903-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-w001-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf32-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mf601-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-mfx32-modem))
$(eval $(call BuildPackage,qcom-msm8916-openstick-wf2-modem))
