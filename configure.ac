#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_PREREQ([2.69])
AC_INIT([ipbt], [6.66], [anakin@pobox.com])
AC_CONFIG_SRCDIR([src/puttyps.h])
AC_CONFIG_HEADERS([uxconfig.h])

AM_INIT_AUTOMAKE

# Checks for programs.
AC_PROG_CC
AC_PROG_CC_C99
AC_PROG_INSTALL

# Checks for libraries.
AC_SEARCH_LIBS(log, m)

# Checks for header files.
AC_CHECK_HEADERS([limits.h locale.h stddef.h stdlib.h string.h sys/ioctl.h sys/time.h termios.h unistd.h wchar.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_TYPE_SIZE_T
AC_TYPE_UID_T

# Checks for library functions.
#AC_FUNC_ERROR_AT_LINE
#AC_FUNC_MALLOC
#AC_FUNC_MBRTOWC
#AC_FUNC_REALLOC
AC_CHECK_FUNCS([endpwent gettimeofday memmove memset select setlocale strchr strerror strstr strtol strtoul])
AC_CHECK_LIB(ncurses, waddch)

AC_CONFIG_FILES([Makefile
		 doc/Makefile
                 src/Makefile])
AC_OUTPUT
