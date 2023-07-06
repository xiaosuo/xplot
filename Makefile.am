#
# Makefile.am for xplot
#
# This software is being provided to you, the LICENSEE, by the
# Massachusetts Institute of Technology (M.I.T.) under the following
# license.  By obtaining, using and/or copying this software, you agree
# that you have read, understood, and will comply with these terms and
# conditions:
# 
# Permission to use, copy, modify and distribute, including the right to
# grant others the right to distribute at any tier, this software and
# its documentation for any purpose and without fee or royalty is hereby
# granted, provided that you agree to comply with the following
# copyright notice and statements, including the disclaimer, and that
# the same appear on ALL copies of the software and documentation,
# including modifications that you make for internal use or for
# distribution:
# 
# Copyright 1992,1993 by the Massachusetts Institute of Technology.
#                     All rights reserved.
# 
# THIS SOFTWARE IS PROVIDED "AS IS", AND M.I.T. MAKES NO REPRESENTATIONS
# OR WARRANTIES, EXPRESS OR IMPLIED.  By way of example, but not
# limitation, M.I.T. MAKES NO REPRESENTATIONS OR WARRANTIES OF
# MERCHANTABILITY OR FITNESS FOR ANY PARTICULAR PURPOSE OR THAT THE USE
# OF THE LICENSED SOFTWARE OR DOCUMENTATION WILL NOT INFRINGE ANY THIRD
# PARTY PATENTS, COPYRIGHTS, TRADEMARKS OR OTHER RIGHTS.
# 
# The name of the Massachusetts Institute of Technology or M.I.T. may
# NOT be used in advertising or publicity pertaining to distribution of
# the software.  Title to copyright in this software and any associated
# documentation shall at all times remain with M.I.T., and USER agrees
# to preserve same.
#

bin_PROGRAMS = xplot tcpdump2xplot

xplot_SOURCES = xplot.c \
		coord.c \
		unsigned.c \
		signed.c \
		timeval.c \
		double.c \
		dtime.c

tcpdump2xplot_SOURCES = tcpdump2xplot.pl

noinst_HEADERS = coord.h \
		 xplot.h

EXTRA_DIST = tcpdump2xplot.pl \
	     ANNOUNCE \
	     README \
	     README.tcp_plots

dist_man1_MANS = xplot.1 \
	     tcpdump2xplot.1

tcpdump2xplot: tcpdump2xplot.pl
	cp -f $(srcdir)/tcpdump2xplot.pl tcpdump2xplot
