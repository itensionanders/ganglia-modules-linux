
DIST_SUBDIRS = example multicpu io fs

AUTOMAKE_OPTIONS = foreign dist-tarZ
ACLOCAL_AMFLAGS = -I m4

if STATIC_BUILD

else

SUBDIRS = example fs multicpu io user

GCFLAGS = -D_LARGEFILE64_SOURCE
GLDFLAGS = -export-dynamic

install:	install-recursive
	@rm -rf $(DESTDIR)$(pkglibdir)/*.a
	@rm -rf $(DESTDIR)$(pkglibdir)/*.la

endif

#EXTRA_DIST = ganglia-gmond-modules.spec

EXTRA_DIST = COPYING gpl-3.0.txt


