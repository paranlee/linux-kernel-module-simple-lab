obj-m += misc_driver.o
MCFLAGS += -std=gnu11
ccflags-y += -Og -ggdb ${MCFLAGS}
CC += ${MCFLAGS}

KDIR = /lib/modules/$(shell uname -r)/build
 
 
all:
	make -C $(KDIR)  M=$(shell pwd) modules
 
clean:
	make -C $(KDIR)  M=$(shell pwd) clean
