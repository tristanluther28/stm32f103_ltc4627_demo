PROJECT = clock
BINARY = clock
BUILD_DIR = bin

SHARED_DIR = ../lib
CFILES = clock.c
CFILES += pwm.c
CFILES += spi.c
CFILES += ltc4627.c

# TODO - you will need to edit these two lines!
DEVICE=stm32f103c4t6a
OOCD_FILE = board/stm32f1x.cfg

# You shouldn't have to edit anything below here.
VPATH += $(SHARED_DIR)
INCLUDES += $(patsubst %,-I%, . $(SHARED_DIR))
OPENCM3_DIR=../libopencm3

include $(OPENCM3_DIR)/mk/genlink-config.mk
include ../rules.mk
include $(OPENCM3_DIR)/mk/genlink-rules.mk
