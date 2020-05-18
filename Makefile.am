
AUTOMAKE_OPTIONS=foreign subdir-objects

bin_PROGRAMS=invoke_server
invoke_server_SOURCES = src/invoke_server.c

COMMON_LIBS = -lubox -lubus

invoke_server_LDADD = $(COMMON_LIBS)

nobase_include_HEADERS = $(wildcard $(top_srcdir)/src/*.h)