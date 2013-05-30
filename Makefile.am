lib_LTLIBRARIES = libxdiff.la

libxdiff_la_LDFLAGS = -version-info $(LIBXDIFF_LIBRARY_VERSION)

libxdiff_includedir = $(includedir)/xdiff

libxdiff_la_SOURCES = xdiffi.c xemit.c xhistogram.c xmerge.c xpatience.c xprepare.c xutils.c

libxdiff_include_HEADERS = xdiff.h xdiffi.h xemit.h xinclude.h xmacros.h xprepare.h xtypes.h xutils.h config.h

pkgconfigdir = $(libdir)/pkgconfig
pkgconfig_DATA = libxdiff.pc

ACLOCAL_AMFLAGS = -I m4
