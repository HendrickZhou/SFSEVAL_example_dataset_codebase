CFLAGS = -g -I

LIBRARY = -lm

#
# section containing definitions of dependencies.
#
multigrid = multigrid.o readimg.o create_image.o GSI.o calc_C.o interp.o residual.o rstrct.o load_depth.o inverse.o GSI2.o

#
# section containing rules to link programs.
#
multigrid:	${multigrid}
	cc -I${INCLUDE} ${CFLAGS} -o $@ ${multigrid} $(LIBRARY)

#
# section containing rules to build object modules (.o's)
#
multigrid.o:	multigrid.c DEF.h

GSI.o:	GSI.c DEF.h

calc_C.o:	calc_C.c DEF.h

interp.o:	interp.c

residual.o:	residual.c DEF.h

rstrct.o:	rstrct.c

readimg.o:	readimg.c DEF.h

create_image.o:	create_image.c DEF.h

load_depth.o:	load_depth.c

GSI2.o:		GSI2.c DEF.h

