AC_INIT([libxdiff], [1.0], [spot@fedoraproject.org])
AC_CONFIG_MACRO_DIR([m4])
AC_CANONICAL_SYSTEM
AM_CONFIG_HEADER(config.h)
AM_INIT_AUTOMAKE([dist-zip])
AC_PROG_CC
AC_PROG_CXX
AM_PROG_AS
AM_PROG_LIBTOOL
LIBTOOL="$LIBTOOL --silent"
AC_PROG_INSTALL
AC_DEFINE(PRODUCTION_BUILD, 1, [Build as a production build])
AC_DEFINE(PRODUCTION, 1, [Build as a production build])
AC_DEFINE(POSIX, 1, [If we're using configure, we're on POSIX])

LIBXDIFF_MAJORMINOR=1.0
AC_SUBST(LIBXDIFF_MAJORMINOR)

LIBXDIFF_LIBRARY_VERSION=1:0:0
AC_SUBST(LIBXDIFF_LIBRARY_VERSION)

AC_C_BIGENDIAN

dnl --------------------------------------------------
dnl only use XDL_FAST_HASH on little-endian
dnl --------------------------------------------------
if test "$ac_cv_c_bigendian" = yes ; then
	XDL_FAST_HASH=0
else
	XDL_FAST_HASH=1
fi
AC_DEFINE_UNQUOTED(XDL_FAST_HASH,$XDL_FAST_HASH,[Define XDL_FAST_HASH on little-endian platforms])

AC_CONFIG_FILES([libxdiff.pc])

AC_OUTPUT([Makefile])
