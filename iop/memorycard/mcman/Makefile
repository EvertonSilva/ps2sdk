#  _____     ___ ____ 
#   ____|   |    ____|      PS2 Open Source Project
#  |     ___|   |____       
#  
#--------------------------------------------------------------------------
#
#    makefile
#
#--------------------------------------------------------------------------

IOP_OBJS_DIR = obj/
IOP_BIN_DIR = bin/
IOP_SRC_DIR = src/
IOP_INC_DIR = include/

IOP_BIN  = bin/mcman.irx
IOP_OBJS = \
obj/main.o obj/mcdev.o obj/mcsio2.o \
obj/ps2mc_fio.o obj/ps1mc_fio.o\
obj/imports.o obj/exports.o

IOP_CFLAGS  += -Wall -fno-builtin -D_IOP #-DSIO_DEBUG #-DDEBUG
IOP_LDFLAGS += -s

all: $(IOP_OBJS_DIR) $(IOP_BIN_DIR) $(IOP_BIN)

clean:
	rm -f -r $(IOP_OBJS_DIR) $(IOP_BIN_DIR)

include $(PS2SDKSRC)/Defs.make
include $(PS2SDKSRC)/iop/Rules.make
include $(PS2SDKSRC)/iop/Rules.release
