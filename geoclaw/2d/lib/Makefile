
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

# Note: This version uses dynamic memory allocation from f90 and so requires
# an f90 compiler such as gfortran.

# Environment variable FC should be set to fortran compiler, e.g. gfortran
FC ?= gfortran44   # default if not set as environment variable

# Add any desired compiler flags such as -g here:
FFLAGS ?= -O2

GEOCLAW_LIB = $(shell pwd)
CLAW_LIB = $(CLAW)/amrclaw/2d/lib/

CLAW_SOURCES = \
  $(GEOCLAW_LIB)/geoclaw_mod.f90 \
  $(GEOCLAW_LIB)/topo_mod.f90 \
  $(GEOCLAW_LIB)/dtopo_mod.f90 \
  $(GEOCLAW_LIB)/qinit_mod.f90 \
  $(GEOCLAW_LIB)/auxinit_mod.f90 \
  $(GEOCLAW_LIB)/allowflag_geo.f \
  $(GEOCLAW_LIB)/amr2ez_geo.f \
  $(GEOCLAW_LIB)/b4step2_geo.f \
  $(GEOCLAW_LIB)/bc2amr_geo.f \
  $(GEOCLAW_LIB)/bilinearintegral_geo.f \
  $(GEOCLAW_LIB)/cellgridintegrate_geo.f \
  $(GEOCLAW_LIB)/dumpgauge_geo.f \
  $(GEOCLAW_LIB)/fgridinterp_geo.f \
  $(GEOCLAW_LIB)/fgridout_geo.f \
  $(GEOCLAW_LIB)/filpatch_geo.f \
  $(GEOCLAW_LIB)/filval_geo.f \
  $(GEOCLAW_LIB)/flag2refine_geo.f \
  $(GEOCLAW_LIB)/flux2fw_geo.f \
  $(GEOCLAW_LIB)/gfixup_geo.f \
  $(GEOCLAW_LIB)/ginit_geo.f \
  $(GEOCLAW_LIB)/movetopo_geo.f \
  $(GEOCLAW_LIB)/qinit_geo.f \
  $(GEOCLAW_LIB)/riemannsolvers_geo.f \
  $(GEOCLAW_LIB)/rpn2ez_fast_geo.f \
  $(GEOCLAW_LIB)/rpn2ez_geo.f \
  $(GEOCLAW_LIB)/rpn2ez_ptwise_geo.f \
  $(GEOCLAW_LIB)/rpn2_geo.f \
  $(GEOCLAW_LIB)/rpt2_geo.f \
  $(GEOCLAW_LIB)/rpt2_ptwise_geo.f \
  $(GEOCLAW_LIB)/setaux_geo.f \
  $(GEOCLAW_LIB)/setfixedgrids_geo.f \
  $(GEOCLAW_LIB)/setgauges_geo.f \
  $(GEOCLAW_LIB)/setgrd_geo.f \
  $(GEOCLAW_LIB)/setprob_geo.f \
  $(GEOCLAW_LIB)/setregions_geo.f \
  $(GEOCLAW_LIB)/src1d_geo.f \
  $(GEOCLAW_LIB)/src2_geo.f \
  $(GEOCLAW_LIB)/step2_geo.f \
  $(GEOCLAW_LIB)/stepgrid_geo.f \
  $(GEOCLAW_LIB)/tick_geo.f \
  $(GEOCLAW_LIB)/topointegral_geo.f \
  $(GEOCLAW_LIB)/upbnd_geo.f \
  $(GEOCLAW_LIB)/update_geo.f \
  $(GEOCLAW_LIB)/valout_geo.f \
  $(GEOCLAW_LIB)/getmaxspeed_geo.f


default: .objs

#-------------------------------------------------------------------
# Include Makefile containing standard definitions and make options:
include $(CLAWMAKE)


### DO NOT remove this line - make depends on it ###

