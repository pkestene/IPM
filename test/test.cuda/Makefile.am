#SUFFIXES = .cu
#include $(top_srcdir)/am/cuda.am

EXTRA_CUDA_LDFLAGS=
if ENABLE_PAPI
EXTRA_CUDA_LDFLAGS += -L$(PAPI_ROOT)/lib -lpapi
endif

#CCC = nvcc -arch sm_20
CCC = nvcc 
SOURCE = main.cu
include $(top_srcdir)/test/Makefile_c

