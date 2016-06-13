## TWRP device tree for Galaxy Note Edge (Europe, China, Oceanic, and Americas)

Add to `.repo/local_manifests/tblte.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/tblte" name="android_device_samsung_tblte" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_tblte-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/nethunter_kernel_trlte/tree/twrp-5.1

