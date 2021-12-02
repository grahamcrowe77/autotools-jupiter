bin_PROGRAMS = jupiter
jupiter_SOURCES = main.c
jupiter_CPPFLAGS = -I$(top_srcdir)/include
jupiter_LDADD = $(top_builddir)/libjup/libjupiter.la

check_SCRIPTS = greptest.sh
TESTS = $(check_SCRIPTS)

greptest.sh:
	echo './jupiter | grep "Hello from .*jupiter!"' > $@
	chmod +x $@

CLEANFILES = greptest.sh
