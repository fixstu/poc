DEBUG_FLAGS =
OPTI_FLAGS =
if PROFILING
DEBUG_FLAGS += -p
endif
if DEBUG
DEBUG_FLAGS += -g3
OPTI_FLAGS += -O0
else
DEBUG_FLAGS += -g
OPTI_FLAGS += -O3
endif

AM_CXXFLAGS = $(WARNINGCFLAGS) $(DEBUG_FLAGS) $(OPTI_FLAGS) -std=c++11

bin_PROGRAMS = poc-multiphase_lock
# 컴파일할 소스.
poc_multiphase_lock_SOURCES =\
  Globals.cpp\
  main.cpp

poc_multiphase_lock_LDFLAGS = -lpthread
