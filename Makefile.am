noinst_LIBRARIES = common/libjupcommon.a
common_libjupcommon_a_SOURCES = common/jupcommon.h common/print.c

bin_PROGRAMS = src/jupiter
src_jupiter_SOURCES = src/main.c
src_jupiter_CPPFLAGS = -I$(top_srcdir)/common
src_jupiter_LDADD = common/libjupcommon.a

check_SCRIPTS = src/greptest.sh
TESTS = $(check_SCRIPTS)

src/greptest.sh:
	echo './src/jupiter | grep "Hello from .*jupiter!"' > $@
	chmod +x $@

CLEANFILES = src/greptest.sh
