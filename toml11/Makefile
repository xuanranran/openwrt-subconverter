# SPDX-License-Identifier: GPL-3.0-only
#
# Copyright (C) 2021 ImmortalWrt.org

include $(TOPDIR)/rules.mk

PKG_NAME:=toml11
PKG_VERSION:=4.0.0
PKG_RELEASE:=1

PKG_SOURCE:=$(PKG_NAME)-$(PKG_VERSION).tar.gz
PKG_SOURCE_URL:=https://codeload.github.com/ToruNiina/toml11/tar.gz/v$(PKG_VERSION)?
PKG_HASH:=f3dc3095f22e38745a5d448ac629f69b7ee76d2b3e6d653e4ce021deb7f7266e

PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

PKG_BUILD_PARALLEL:=1
CMAKE_INSTALL:=1

include $(INCLUDE_DIR)/package.mk
include $(INCLUDE_DIR)/cmake.mk

define Package/toml11
  SECTION:=lib
  CATEGORY:=Libraries
  TITLE:=C++11 header-only toml parser/encoder
  URL:=https://github.com/ToruNiina/toml11
endef

define Package/toml11/description
  toml11 is a C++11 (or later) header-only toml parser/encoder
  depending only on C++ standard library.
endef

$(eval $(call BuildPackage,toml11))
