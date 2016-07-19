STATIC_PATH := staticlib
SHARED_PATH := sharedlib 


all: build install
	@echo "Enter `pwd` all"

build:
	@echo "Enter `pwd` build"
	$(MAKE) -C $(STATIC_PATH) build
	#$(MAKE) -C $(SHARED_PATH) build

install:
	@echo "Enter `pwd` install"
	$(MAKE) -C $(STATIC_PATH) install 
	#$(MAKE) -C $(SHARED_PATH) install

clean:
	@echo "Enter `pwd` clean"
	$(MAKE) -C $(STATIC_PATH) clean 
	#$(MAKE) -C $(SHARED_PATH) clean
