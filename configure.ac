dnl Process this file with autoconf to produce a configure script.
AC_INIT([xplot], [0.90.7.1])
AC_CONFIG_SRCDIR([xplot.c])
AC_CONFIG_HEADERS([config.h])
AM_INIT_AUTOMAKE

dnl Checks for programs.
AC_PROG_CC
if test $ac_cv_c_compiler_gnu = yes; then
  CFLAGS="$CFLAGS -Wall"
fi

AC_PROG_INSTALL

dnl Find X11, and add the include/libs to the c/ld flags
dnl This must be done BEFORE checking for the X libraries
AC_PATH_XTRA
LIBS="$LIBS $X_LIBS"
CFLAGS="$CFLAGS $X_CFLAGS"

dnl Checks for libraries.
dnl Replace `main' with a function in -lX11:
AC_CHECK_LIB(X11, main)
dnl Replace `main' with a function in -lm:
AC_CHECK_LIB(m, main)

dnl Checks for typedefs, structures, and compiler characteristics.
AC_C_INLINE

AC_STRUCT_TM

dnl Checks for library functions.

AC_CONFIG_FILES([Makefile])
AC_OUTPUT

