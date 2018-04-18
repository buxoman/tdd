#---------
#
# CppUTest Examples Makefile
#
#----------

#Set this to @ to keep the makefile quiet
ifndef SILENCE
	SILENCE = @
endif

#--- Inputs ----#
COMPONENT_NAME = erase_repeated_chars
CPPUTEST_HOME = ../../../cpputest

CPPUTEST_ENABLE_DEBUG = Y
CPPUTEST_USE_LONG_LONG = Y
CPPUTEST_USE_GCOV = Y
CPPUTEST_USE_EXTENSIONS = Y
CPP_PLATFORM = Gcc
CPPUTEST_CXXFLAGS += -std=c++11

# This line is overriding the default new macros.  This is helpful
# when using std library includes like <list> and other containers
# so that memory leak detection does not conflict with stl.
#CPPUTEST_MEMLEAK_DETECTOR_NEW_MACRO_FILE = -include ApplicationLib/ExamplesNewOverrides.h
SRC_DIRS = \
	ApplicationLib

TEST_SRC_DIRS = \
	AllTests

INCLUDE_DIRS =\
  .\
  ApplicationLib\
  $(CPPUTEST_HOME)/include\

include $(CPPUTEST_HOME)/build/MakefileWorker.mk


