APP_PATH := app
COMMON_PATH := commonapi 


all: build install
	@echo "Enter `pwd` all"

build:
	@echo "Enter `pwd` build"
	$(MAKE) -C $(APP_PATH) build
	$(MAKE) -C $(COMMON_PATH) build

install:
	@echo "Enter `pwd` install"
	$(MAKE) -C $(APP_PATH) install 
	$(MAKE) -C $(COMMON_PATH) install

clean:
	@echo "Enter `pwd` clean"
	$(MAKE) -C $(APP_PATH) clean 
	$(MAKE) -C $(COMMON_PATH) clean
