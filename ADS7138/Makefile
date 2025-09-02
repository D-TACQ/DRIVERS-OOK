
# pgm : clone from drivers/iio/adc/ti-ads7138.c

obj-m += ti-ads7138.o

all:
	make -C $(KERN_SRC) ARCH=arm M=`pwd` modules

modules: $(obj-m)

zynq:
	./make.zynq

clean:
	rm -f *.ko *.o *.mod.* modules.order Module.symvers



