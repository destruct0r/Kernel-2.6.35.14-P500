#
# Makefile for the Linux unix domain socket layer.
#

obj-$(CONFIG_UNIX)	+= unix.o

unix-y			:= af_unix.o garbage.o
unix-$(CONFIG_SYSCTL)	+= sysctl_net_unix.o

# Ignore warnings to prevent build breaks
CFLAGS_REMOVE_af_unix.o = -Werror
