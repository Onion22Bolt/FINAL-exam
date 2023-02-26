obj-m += usb-driver.o

KERNEL_DIR += /lib/modules/$(shell uname -r)/build

all:
	$(MAKE) -C $(KERNEL_DIR) M=$(shell pwd) modules
clean:
	sudo rm -rf *.o *.ko *.mod.c *.order *.symvers *.mod .usb* .modules* .Module*
.PHONY:clean