CM13.0 Kernel for DUMA

This is a Ported CyanogenMod Kernel from Nexus 7 2013 (flo/deb)
This kernel is full working, with some extra features:

- ExFat Support (thanks to SevenMaxs)
- External SD support
- Fast Charge support (thanks to SevenMaxs)

List of modified files in the flo/deb kernel:

arch/arm/mach-msm/asustek/duma/*   (build duma board files comparing ASUS JB kernel source with flo board files from cm13 kernel)
arch/arm/mach-msm/asustek/Kconfig.board
arch/arm/mach-msm/asustek/Makefile.board
arch/arm/mach-msm/asustek/asustek-pcbid.c
arch/arm/mach-msm/perf_trace_counters.h
arch/arm/mach-msm/restart.c
drivers/mfd/pm8xxx-pwm.c
drivers/input/touchscreen/ektf3.c  (backport from ASUS JB Kernel for DUMA)	
drivers/input/touchscreen/fw_data.b (backport from ASUS JB Kernel for DUMA)
drivers/input/touchscreen/Kconfig
drivers/media/platform/msm/camera2/sensor/mi1040.c
drivers/media/platform/msm/camera2/sensor/msm_sensor.c
drivers/power/bq27541_battery.c
drivers/smb345-charger.c
drivers/usb/otg/msm_otg.c
drivers/video/msm/Kconfig
drivers/video/msm/Makefile
drivers/video/msm/mdp.c
drivers/video/msm/mdp4.h
drivers/video/msm/mipi_dsi.c
drivers/video/msm/mipi_orise.c
drivers/video/msm/mipi_auo_video_1080P.c
arch/arm/tools/mach-types
sound/soc/msm/apq8064.c
sound/soc/msm/apq8064-i2s.c
sound/soc/msm/asustek_headset.c
include/linux/pwm.h
include/linux/slimport.h
include/linux/i2c/ektf3k.h

For fastcharge patch:
include/linux/fastch.h
arch/arm/mach-msm/Kconfig
arch/arm/mach-msm/Makefile
arch/arm/mach-msm/fastchg.c

