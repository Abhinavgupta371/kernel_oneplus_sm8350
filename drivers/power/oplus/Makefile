ifeq ($(CONFIG_OPLUS_CHARGER_MTK),y)
subdir-ccflags-y += -Werror
subdir-ccflags-y += -Wno-unused-variable
ifeq ($(CONFIG_OPLUS_CHARGER_MTK6779Q),y)
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include
endif
endif
ifeq ($(CONFIG_OPLUS_CHARGER_MTK6889),y)
subdir-ccflags-y += -I$(srctree)/drivers/misc/mediatek/include
endif
ifneq ($(CONFIG_OPLUS_CHARGER_MTK),y)
obj-y      += wireless_ic/
endif
obj-y      += charger_ic/
obj-y      += gauge_ic/
obj-y      += warp_ic/
obj-y      += adapter_ic/

obj-y	+= oplus_charger.o
obj-y	+= oplus_gauge.o
obj-y	+= oplus_warp.o
obj-y	+= oplus_adapter.o
obj-y	+= oplus_wireless.o
obj-y	+= oplus_short.o
obj-y   += oplus_debug_info.o
obj-y   += oplus_chg_ops_manager.o

obj-y   += oplus_pps.o