
# Library version of Makefile
# ---------------------------

# Only "make .objs" and "make .htmls" are useful in this directory.

# Makefile for Clawpack code in this directory.
# This version only sets the local files and frequently changed
# options, and then includes the standard makefile pointed to by CLAWMAKE.
CLAWMAKE = $(CLAW)/util/Makefile.common

# See the above file for details and a list of make options, or type
#   make .help
# at the unix prompt.


# Environment variable FC should be set to fortran compiler, e.g. gfortran
FC ?= gfortran   # default if not set as environment variable
# Add any desired compiler flags such as -g here:
FFLAGS ?=

CLAW_LIB = $(shell pwd)

CLAW_SOURCES = \
  $(CLAW_LIB)/gauges_mod.f90 \
  $(CLAW_LIB)/setprob_geo.f \
  $(CLAW_LIB)/setswparams_geo.f \
  $(CLAW_LIB)/bc1_geo.f \
  $(CLAW_LIB)/b4step1_geo.f \
  $(CLAW_LIB)/novaccum1_geo.f \
  $(CLAW_LIB)/src1_geo.f \
  $(CLAW_LIB)/out1_geo.f \
  $(CLAW_LIB)/riemannsolvers_geo.f \
  $(CLAW_LIB)/rp1ez_geo.f \
  $(CLAW_LIB)/rp1_geo.f \
  $(CLAW_LIB)/opendatafile_geo.f \
  $(CLAW_LIB)/step1fw_geo.f \

default: .objs


#-------------------------------------------------------------------
# Include Makefile containing standard definitions and make options:
include $(CLAWMAKE)


### DO NOT remove this line - make depends on it ###

