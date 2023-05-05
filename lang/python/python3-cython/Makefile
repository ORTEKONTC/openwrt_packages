#
# This is free software, licensed under the GNU General Public License v2.
# See /LICENSE for more information.
#

include $(TOPDIR)/rules.mk

PKG_NAME:=Cython
PKG_VERSION:=0.29.34
PKG_RELEASE:=14
PKG_LICENSE:=BSD-3-Clause

PYPI_NAME:=$(PKG_NAME)
PKG_HASH:=1909688f5d7b521a60c396d20bba9e47a1b2d2784bfb085401e1e1e7d29a29a8

include ../pypi.mk
include $(INCLUDE_DIR)/package.mk
include ../python3-package.mk

define Package/python3-cython
  SUBMENU:=Python
  SECTION:=lang
  CATEGORY:=Languages
  TITLE:=Cython
  URL:=https://www.cython.org
  DEPENDS:=+python3
endef

define Package/python3-cython/description
  Cython is a language that should make writing C extensions for the Python language easier
endef

$(eval $(call Py3Package,python3-cython))
$(eval $(call BuildPackage,python3-cython))
$(eval $(call BuildPackage,python3-cython-src))
