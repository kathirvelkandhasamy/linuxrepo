obj-m+=char_dev.o
 
all:
	make -C /lib/modules/$(shell uname -r)/build/ M=$(PWD) modules
	$(CC) userspacefile.c -o usrfile

clean:
	make -C /lib/modules/$(shell uname -r)/build/ M=$(PWD) clean
	rm usrfile