#export ROOT_PATH := `pwd`
#PWD := `pwd`
#PWD = `pwd` #用這個會把pwd執行動作帶到下一個Makefile
PWD = $(shell pwd) #用這個才能真的抓到當下的位置
#export ROOT_PATH=$(PWD) #用這種方式對於sub-makefile的參數取用會多一個空格
export ROOT_PATH=$(shell pwd)
APP_PATH := app
COMMON_PATH := commonapi 


all: build install
	@echo "Enter `pwd` all"

build:
	@echo "Enter `pwd` build"
	@echo "**********ROOT_PATH is $(ROOT_PATH)"
	$(MAKE) -C $(COMMON_PATH) build
	$(MAKE) -C $(APP_PATH) build

install:
	@echo "Enter `pwd` install"
	$(MAKE) -C $(COMMON_PATH) install
	$(MAKE) -C $(APP_PATH) install 

clean:
	@echo "Enter `pwd` clean"
	$(MAKE) -C $(COMMON_PATH) clean
	$(MAKE) -C $(APP_PATH) clean 
