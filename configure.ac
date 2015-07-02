#                                               -*- Autoconf -*-
# Process this file with autoconf to produce a configure script.

AC_INIT([hintsvm], [0.1], [https://github.com/yangarbiter/hintsvm])
AC_CONFIG_SRCDIR([svm.h])
AC_CONFIG_HEADERS([config.h])

AM_INIT_AUTOMAKE([foreign])

# Checks for programs.
AC_PROG_CXX
AC_PROG_CC
AC_PROG_MAKE_SET
AC_PROG_CC_STDC
AC_PROG_RANLIB
AC_PROG_LIBTOOL
AM_PATH_PYTHON([3])
if test x"${ac_cv_prog_cc_c99}" = xno; then
    AC_MSG_ERROR([C99 support is required to compile $PACKAGE])
fi

# Checks for libraries.
AC_SEARCH_LIBS([tanh], [m])

# Checks for header files.
AC_CHECK_HEADERS([float.h limits.h stdlib.h string.h])

# Checks for typedefs, structures, and compiler characteristics.
AC_CHECK_HEADER_STDBOOL
AC_C_INLINE

# Checks for library functions.
AC_FUNC_MALLOC
AC_FUNC_REALLOC
AC_FUNC_STRTOD
AC_CHECK_FUNCS([sqrt strrchr strtol])

AM_SILENT_RULES([yes])

AC_CONFIG_FILES([Makefile])
AC_OUTPUT
