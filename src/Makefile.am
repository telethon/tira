ACLOCAL_AMFLAGS = -I m4
bin_PROGRAMS = ipbt
ipbt_SOURCES = be_none.c fromucs.c ipbt.c ldiscucs.c localenc.c macenc.c \
       mimeenc.c minibidi.c misc.c noprint.c notiming.c sbcs.c sbcsdat.c \
       settings.c slookup.c terminal.c time.c toucs.c tree234.c utf8.c \
       uxmisc.c uxucs.c wcwidth.c xenc.c
ipbt_LDADD = $(LIBOBJS)

EXTRA_DIST = puttyps.h puttymem.h putty.h unix.h charset.h charset.h \
	enum.c internal.h ldisc.h mimeenc.c minibidi.c misc.c misc.h \
	putty.h puttymem.h puttyps.h sbcs.dat sbcsgen.pl settings.c \
	terminal.c terminal.h time.c tree234.c tree234.h network.h \
	storage.h

BUILT_SOURCES = sbcsdat.c
sbcsdat.c: sbcsgen.pl sbcs.dat
	perl $(srcdir)/sbcsgen.pl $(srcdir)/sbcs.dat
