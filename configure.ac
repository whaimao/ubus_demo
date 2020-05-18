#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT(invoke_server, 0.0.1, ganjianxuan@hotmail.com)
AM_INIT_AUTOMAKE
AC_CONFIG_SRCDIR([src/invoke_server.c])
AC_CONFIG_HEADERS([config.h])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_RANLIB

# Checks for libraries.
# FIXME: Replace `main' with a function in `-lpthread':
AC_CHECK_LIB([pthread], [pthread_create])

#AC_DEFUN([CURL_FAIL], [
#  AC_MSG_FAILURE([please the curl library in the target system])
#])
AC_CHECK_LIB([curl], [curl_easy_init], [true], [])

# Checks for header files.
AC_FUNC_ALLOCA
AC_CHECK_HEADERS([arpa/inet.h fcntl.h float.h limits.h mach/mach.h malloc.h netdb.h netinet/in.h stddef.h stdint.h stdlib.h string.h strings.h sys/file.h sys/ioctl.h sys/socket.h sys/time.h sys/timeb.h unistd.h wchar.h wctype.h pthread.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE
AC_TYPE_INT32_T
AC_TYPE_INT64_T
AC_TYPE_PID_T
AC_TYPE_SIZE_T
AC_TYPE_SSIZE_T
AC_TYPE_UINT32_T
AC_TYPE_UINT64_T
AC_CHECK_TYPES([ptrdiff_t])

# Checks for library functions.
AC_FUNC_ERROR_AT_LINE
AC_FUNC_FORK
AC_FUNC_MALLOC
AC_FUNC_MKTIME
AC_FUNC_MMAP
AC_FUNC_REALLOC
AC_FUNC_STRERROR_R
AC_CHECK_FUNCS([clock_gettime dup2 fchdir getcwd getpagesize gettimeofday memmove memset mkdir modf munmap regcomp rmdir select socket strcasecmp strchr strdup strerror strncasecmp strpbrk strrchr strstr strtol strtoul strtoull, pread])


AC_CONFIG_FILES([Makefile])
AC_OUTPUT
