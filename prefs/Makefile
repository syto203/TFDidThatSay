include $(THEOS)/makefiles/common.mk

ARCHS = armv7 armv7s arm64 arm64e

BUNDLE_NAME = TFDidThatSayPrefs

TFDidThatSayPrefs_FILES = TFDTSRootListController.m
TFDidThatSayPrefs_INSTALL_PATH = /Library/PreferenceBundles
TFDidThatSayPrefs_FRAMEWORKS = UIKit
TFDidThatSayPrefs_PRIVATE_FRAMEWORKS = Preferences
TFDidThatSayPrefs_CFLAGS = -fobjc-arc -Wno-unguarded-availability-new

include $(THEOS_MAKE_PATH)/bundle.mk

internal-stage::
	$(ECHO_NOTHING)mkdir -p $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences$(ECHO_END)
	$(ECHO_NOTHING)cp entry.plist $(THEOS_STAGING_DIR)/Library/PreferenceLoader/Preferences/TFDidThatSayPrefs.plist$(ECHO_END)
