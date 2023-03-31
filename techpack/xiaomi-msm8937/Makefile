ifeq ($(CONFIG_MACH_XIAOMI_MSM8937),y)
# Use USERINCLUDE when you must reference the UAPI directories only.
USERINCLUDE     += \
                -I$(srctree)/techpack/xiaomi-msm8937/include/uapi \

# Use LINUXINCLUDE when you must reference the include/ directory.
# Needed to be compatible with the O= option
LINUXINCLUDE    += \
                -I$(srctree)/techpack/xiaomi-msm8937/include/uapi \
                -I$(srctree)/techpack/xiaomi-msm8937/include
else
ccflags-y := -Wno-unused-function
obj-y := stub.o
endif
