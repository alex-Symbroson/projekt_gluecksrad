###############################################################################
#                                                                             #
# devel/.../Makefile                                                          #
# ==================                                                          #
#                                                                             #
# Version: 1.0.2                                                              #
# Date   : 07.02.18                                                           #
# Author : Peter Weissig                                                      #
#                                                                             #
# Source code was taken from:                                                 #
#   https://github.com/RoboSAX/avr_spielfeld                                  #
#                                                                             #
# See also:                                                                   #
#   https://github.com/RoboAG/projekt_gluecksrad                              #
###############################################################################

CURRENTDIR = Peter

SUBDIRS = tests/cover tests/leds1 tests/leds2 tests/random

###############################################################################
# define phony targets for make commands
.PHONY: all all_init  $(SUBDIRS)  clean

all: all_init $(SUBDIRS)

all_init:
	@echo "# building $(CURRENTDIR) #"


$(SUBDIRS):
	$(MAKE) -C $@ -f "$(ROBOLIB_MAKEFILE)"


clean:
	@echo
	@echo "# clean $(CURRENTDIR) #"
	@for dir in $(SUBDIRS); do \
	    $(MAKE) -C $$dir -f "$(ROBOLIB_MAKEFILE)" clean; \
	done

###############################################################################
