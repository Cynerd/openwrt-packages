# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=bigclown-control-tool
PKG_VERSION:=1.1.0
PKG_RELEASE:=1

PYPI_NAME:=bch
PKG_HASH:=7af9471c4f9d5593aae2606ea59dcf5f1a1635117dd51d19fb623f8b4080777a

PKG_MAINTAINER:=Karel Kočí <cynerd@email.cz>
PKG_LICENSE:=MIT
PKG_LICENSE_FILES:=LICENSE

include ../../../lang/python/pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../../../lang/python/python3-package.mk

define Package/bigclown-control-tool
  SECTION:=utils
  CATEGORY:=Utilities
  SUBMENU:=BigClown
  TITLE:=BigCLown control tool
  URL:=https://github.com/bigclownlabs/bch-control-tool
  DEPENDS:=\
    +python3-click \
    +python3-click-log \
    +python3-paho-mqtt \
    +python3-pyserial \
    +python3-yaml \
    +python3-simplejson
endef

$(eval $(call Py3Package,bigclown-control-tool))
$(eval $(call BuildPackage,bigclown-control-tool))
