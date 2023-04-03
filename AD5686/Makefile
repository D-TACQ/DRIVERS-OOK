#KERN_SRC=../../linux-xlnx

# pgm derived from:
# meld AD5686/ ../adi-linux/drivers/iio/dac/

obj-m += ad5696-i2c.o
obj-m += ad5686.o

all:
	make -C $(KERN_SRC) ARCH=arm M=`pwd` modules

modules: $(obj-m)

zynq:
	./make.zynq

clean:
	rm -f *.ko *.o *.mod.* modules.order Module.symvers


