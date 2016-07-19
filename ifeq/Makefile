all:
	#執行make之前，在command下執行export CONFIG_N="Nelson"
	#ifeq會成立
	#執行make之前，在command下執行export CONFIG_N="test"
	#else會成立
	#ifeq判斷式裡面，不能用雙引號，or會判斷不對。
ifeq ($(CONFIG_N), Nelson)
	@echo "CONFIG_N is \"I am Nelson\""
else
	@echo "CONFIG_N is $(CONFIG_N)"
endif
	#執行make之前，在command下執行export CONFIG_TEST="\"TEST\""
	#ifeq會成立
	#執行make之前，在command下執行export CONFIG_TEST="test"
	#else會成立
	#此種情況，判斷就要加上雙引號
	#關鍵就是你在使用export的差異
ifeq ($(CONFIG_TEST), "TEST")
	@echo "CONFIG_TEST is \"I am TEST\""
else
	@echo "CONFIG_TEST is $(CONFIG_TEST)"
endif
