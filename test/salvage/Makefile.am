AM_CPPFLAGS = -I$(top_builddir) -I$(top_srcdir)/src/include

noinst_PROGRAMS = t
t_SOURCES = salvage.c
t_LDADD = $(top_builddir)/libwiredtiger.la
t_LDFLAGS = -static

# Run this during a "make check" smoke test.
TESTS = $(noinst_PROGRAMS)

clean-local:
	rm -rf WiredTiger* *.core __*
