## Process this file with autoconf to produce a configure script.

## Copyright © 2008 Keith Packard
## All Rights Reserved.  See the file COPYING in this directory
## for licensing information.

AUTOMAKE_OPTIONS = foreign

NICKLEFILES = \
	ricochet.5c \
	rrboard.5c \
	rrgame.5c \
	rrpiece.5c \
	rrtimer.5c

EXTRA_DIST = $(NICKLEFILES) autogen.sh ricochet.in

pkgdata_DATA = $(NICKLEFILES)

bin_SCRIPTS = ricochet

ricochet: ricochet.in Makefile
	sed -e 's,@''RICOCHET_LIBDIR@,$(RICOCHET_LIBDIR),' \
	$(top_srcdir)/ricochet.in > $@
	chmod +x $@

clean-local:
	rm -f ricochet
