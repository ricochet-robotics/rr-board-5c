dnl Process this file with autoconf to produce a configure script.

dnl Copyright © 2008 Keith Packard
dnl All Rights Reserved.  See the file COPYING in this directory
dnl for licensing information.

AC_PREREQ(2.59)

AC_INIT([ricochet],
	1.0,
	[http://nickle.org],
	ricochet)

AC_CONFIG_SRCDIR([ricochet.5c])
AM_INIT_AUTOMAKE([foreign])
AM_MAINTAINER_MODE

dnl libtool versioning

AC_PROG_INSTALL
AC_PROG_LN_S
AC_PROG_MAKE_SET

RICOCHET_SYS_LIBDIR=`eval echo ${datadir}`/ricochet

AC_ARG_WITH(ricochet-libdir, AS_HELP_STRING([--with-ricochet-libdir=LIBDIR],
				[Directory where nickle source files should be installed (default $RICOCHET_SYS_LIBDIR)]),
			   [ RICOCHET_LIBDIR="$withval" ],
			   [ RICOCHET_LIBDIR="$RICOCHET_SYS_LIBDIR" ])

AC_SUBST(RICOCHET_LIBDIR)

AC_CONFIG_FILES([Makefile])
		
AC_OUTPUT
