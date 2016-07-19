QUIET = @
ECHO = $(QUIET)echo
CC = gcc
FILES = $(wildcard *.c)
OBJS  = $(patsubst %.c,%.o,$(wildcard *.c))

all: build install
	$(ECHO) "Enter `pwd` all"

build: $(OBJS)
	$(ECHO) $(FILES)
	$(ECHO) $(OBJS)
	$(ECHO) "Enter `pwd` build"

%.o: %.c
	$(ECHO) "Compliling " $<
	$(QUIET)$(CC) $(CFLAGS) -c $< -o $@

install:
	@echo "Enter `pwd` install"

clean:
	@echo "Enter `pwd` clean"
	rm *.o

info:
	$(ECHO) "CC = $(CC)"
	$(ECHO) "FILES = $(FILES)"
	$(ECHO) "OBJS = $(OBJS)"
