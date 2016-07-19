HELLO_PATH := app_hello 
HI_PATH := app_hi

all: build install
	@echo "Enter `pwd` all"

build:
	@echo "Enter `pwd` build"
	@echo $(OBJS)
	$(MAKE) -C $(HELLO_PATH) build
	$(MAKE) -C $(HI_PATH) build

install:
	@echo "Enter `pwd` install"

clean:
	@echo "Enter `pwd` clean"
