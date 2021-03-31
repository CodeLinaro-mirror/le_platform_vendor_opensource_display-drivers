# SPDX-License-Identifier: GPL-2.0-only

ifeq ($(DISPLAY_ROOT),)
export DISPLAY_ROOT=$(srctree)/techpack/display
export KERNEL_SRC=$(srctree)
CONFIG_DRM_MSM=y
endif

LINUXINCLUDE    += \
		   -I$(DISPLAY_ROOT)/include/uapi/display \
		   -I$(DISPLAY_ROOT)/include
USERINCLUDE     += -I$(DISPLAY_ROOT)/include/uapi/display

obj-$(CONFIG_DRM_MSM) += msm/
