QUIET = @
ECHO = $(QUIET)echo
CC = gcc
FILES = $(wildcard *.c)
OBJS  = $(patsubst %.c,%.o,$(wildcard *.c))
INCLUDE_FILE = -I$(ROOT_PATH)/commonapi/inc 
LIB_PATH = -L$(ROOT_PATH)/commonapi/lib
STATIC_LIB = -lshow
SHARED_LIB = -l

all: build install
	$(ECHO) "Enter `pwd` all"

build: $(OBJS)
	$(ECHO) $(FILES)
	$(ECHO) $(OBJS)
	$(ECHO) "Enter `pwd` build"

%.o: %.c
	$(ECHO) "Compliling " $<
	#$(QUIET)$(CC) $(CFLAGS) -c $< -o $@
	$(QUIET)$(CC) -static $(INCLUDE_FILE) $(LIB_PATH) $< 

install:
	@echo "Enter `pwd` install"

clean:
	@echo "Enter `pwd` clean"
	rm *.o

info:
	$(ECHO) "CC = $(CC)"
	$(ECHO) "FILES = $(FILES)"
	$(ECHO) "OBJS = $(OBJS)"
