sTHEOS_PACKAGE_DIR_NAME = debs
ARCHS = armv7 armv7s arm64
THEOS_DEVICE_IP = 192.168.33.128
THEOS_DEVICE_PORT=22
FINALPACKAGE = 1
include theos/makefiles/common.mk

TWEAK_NAME = GetOverHere
GetOverHere_FILES = Tweak.xm
GetOverHere_FRAMEWORKS = UIKit

include $(THEOS_MAKE_PATH)/tweak.mk

after-install::
	install.exec "killall -9 MobileMail"
