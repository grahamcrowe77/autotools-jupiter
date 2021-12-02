ACLOCAL_AMFLAGS = -I m4

SUBDIRS = modules/hithere

bin_PROGRAMS = jupiter
jupiter_SOURCES = main.c module.h
jupiter_CPPFLAGS = -I$(top_srcdir)/include
jupiter_LDADD = $(top_builddir)/libjup/libjupiter.la -dlopen modules/hithere/hithere.la
