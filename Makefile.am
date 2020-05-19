
AUTOMAKE_OPTIONS=foreign subdir-objects

bin_PROGRAMS=invoke_server event_server event_client

invoke_server_SOURCES = src/invoke_server.c

event_server_SOURCES = src/event_server.c

event_client_SOURCES = src/event_client.c

COMMON_LIBS = -lubox -lubus -lblobmsg_json

invoke_server_LDADD = $(COMMON_LIBS)
event_server_LDADD = $(COMMON_LIBS)
event_client_LDADD = $(COMMON_LIBS)

nobase_include_HEADERS = $(wildcard $(top_srcdir)/src/*.h)