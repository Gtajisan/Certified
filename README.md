#Android certs for Signing...
**clone**
```
git clone https://github.com/Gtajisan/Certified
```
***apply***
# Have to add these flags in device.mk
```
SIGNING_KEY_PATH ?= Certified
RELEASE_KEY := $(SIGNING_KEY_PATH)/releasekey
SIGNING_KEY_PATH ?= Certified
RELEASE_KEY := $(SIGNING_KEY_PATH)/releasekey
PRODUCT_DEFAULT_DEV_CERTIFICATE := $(RELEASE_KEY)
PRODUCT_OTA_PUBLIC_KEYS := $(RELEASE_KEY)
```
