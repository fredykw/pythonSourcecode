# Generated automatically from Makefile.in by configure.
# NOTE: Makefile.in is converted into Makefile by the configure script
# in the parent directory.  Once configure has run, you can recreate
# the Makefile by running just config.status.

# === Variables set by config.stat ===

VERSION=	2.0

srcdir=		.

CC=		gcc
RANLIB=		ranlib
AR=		ar

DEFS=		-DHAVE_CONFIG_H


# === Other things that are customizable but not by configure ===

INCLDIR=	$(srcdir)/../Include
OPT=		-g -O2 -Wall -Wstrict-prototypes -fPIC
CFLAGS=		$(OPT) -I$(INCLDIR) -I.. $(DEFS)

MKDEP=		mkdep
SHELL=		/bin/sh


# === Fixed definitions ===

OBJS=		abstract.o bufferobject.o \
		classobject.o cobject.o complexobject.o \
		fileobject.o floatobject.o \
		frameobject.o funcobject.o intobject.o listobject.o \
		longobject.o dictobject.o methodobject.o \
		moduleobject.o object.o rangeobject.o \
		sliceobject.o stringobject.o \
		tupleobject.o typeobject.o \
		unicodeobject.o unicodectype.o

SRCS=		abstract.c bufferobject.c \
		classobject.c cobject.c complexobject.c \
		fileobject.c floatobject.c \
		frameobject.c funcobject.c intobject.c listobject.c \
		longobject.c dictobject.c methodobject.c \
		moduleobject.c object.c rangeobject.c \
		sliceobject.c stringobject.c \
		tupleobject.c typeobject.c \
		unicodeobject.c unicodectype.c

LIBRARY=	../libpython$(VERSION).a

# === Rules ===

all:		$(OBJS)

# This target is used by the master Makefile to add the objects to the library
add2lib:	$(OBJS)
		$(AR) cr $(LIBRARY) $(OBJS)
		touch add2lib

clean:
		-rm -f *.o core *~ [@,#]* *.old *.orig *.rej add2lib

clobber:	clean
		-rm -f *.a tags TAGS

Makefile:	$(srcdir)/Makefile.in ../config.status
		(cd ..; CONFIG_FILES=Objects/Makefile CONFIG_HEADERS= \
		$(SHELL) config.status)

depend:
		$(MKDEP) $(CFLAGS) `echo $(OBJS) | tr ' ' '\012' | \
					sed 's|\(.*\)\.o|$(srcdir)/\1.c|'`

.PRECIOUS:	Makefile

abstract.o: abstract.c
bufferobject.o: bufferobject.c
classobject.o: classobject.c
cobject.o: cobject.c
complexobject.o: complexobject.c
fileobject.o: fileobject.c
floatobject.o: floatobject.c
frameobject.o: frameobject.c
funcobject.o: funcobject.c
intobject.o: intobject.c
listobject.o: listobject.c
longobject.o: longobject.c
dictobject.o: dictobject.c
methodobject.o: methodobject.c
moduleobject.o: moduleobject.c
object.o: object.c
rangeobject.o: rangeobject.c
sliceobject.o: sliceobject.c
stringobject.o: stringobject.c
tupleobject.o: tupleobject.c
typeobject.o: typeobject.c
unicodeobject.o: unicodeobject.c
unicodectype.o: unicodectype.c

# DO NOT DELETE THIS LINE -- mkdep uses it.
# DO NOT PUT ANYTHING AFTER THIS LINE, IT WILL GO AWAY.
# IF YOU PUT ANYTHING HERE IT WILL GO AWAY
