
# pgm : clone from drivers/iio/adc/ti-ads7138.c

obj-m += ti-ads7138.o

all:
	make -C $(KERN_SRC) ARCH=arm M=`pwd` modules
	dtc -@ -I dts -O dtb -o octobee-ads7128.dtb octobee-ads7128.dts

modules: $(obj-m)

zynq:
	./make.zynq

clean:
	rm -f *.ko *.o *.mod.* modules.order Module.symvers



