#Ref: http://www.adp-gmbh.ch/cpp/gcc/create_lib.html
LIB_H_FILE=$(wildcard *.h)
LIB_C_FILE=$(wildcard *.c)
LIB_O_FILE=$(wildcard *.o)
LIB_NAME=show

all: build install
	@echo "Enter `pwd` all"

build:
	#ld fail
	#gcc -static $(LIB_C_FILE) -l$(LIB_NAME)
	#gcc -v -static $(LIB_C_FILE) -o lib$(LIB_NAME).a
	#It is ok
	gcc $(LIB_C_FILE) -c
	ar rsv lib$(LIB_NAME).a $(LIB_O_FILE) 
	@echo "Enter `pwd` build"

install:
	@echo "Enter `pwd` install"
	@echo "===ROOT_PATH is $(ROOT_PATH)"
	#@echo "===cp lib$(LIB_NAME).a $(ROOT_PATH)/commonapi/lib"
	@cp lib$(LIB_NAME).a $(ROOT_PATH)/commonapi/lib
	@cp $(LIB_H_FILE) $(ROOT_PATH)/commonapi/inc

clean:
	@echo "Enter `pwd` clean"
	#rm $(LIB_O_FILE) lib$(LIB_NAME).a ../lib/lib$(LIB_NAME).a
	rm $(LIB_O_FILE) lib$(LIB_NAME).a $(ROOT_PATH)/commonapi/lib/lib$(LIB_NAME).a
