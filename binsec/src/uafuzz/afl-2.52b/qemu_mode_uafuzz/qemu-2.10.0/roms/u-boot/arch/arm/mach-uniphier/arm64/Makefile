#
# SPDX-License-Identifier:	GPL-2.0+
#

ifdef CONFIG_SPL_BUILD
obj-y += timer.o
else
obj-y += mem_map.o
ifdef CONFIG_ARMV8_MULTIENTRY
obj-y += smp.o smp_kick_cpus.o
obj-$(CONFIG_ARCH_UNIPHIER_LD20) += arm-cci500.o
else
obj-$(CONFIG_ARCH_UNIPHIER_LD20) += lowlevel_init.o
endif
endif
