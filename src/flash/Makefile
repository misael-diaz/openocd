#!/usr/bin/make
#
# openocd-fork			November 21, 2026
#
# source: Makefile
# author: @misael-diaz
#
# Synopsis:
# Defines the Makefile for building the program with GNU make.
#
# Copyright (c) 2026 Misael Díaz-Maldonado
#
# This file is released under the GNU General Public License version 2 only
# as published by the Free Software Foundation.
#

include make-inc

all: $(OBJS) 

$(COMMON_O): $(COMMON_C)
	$(CC) $(CCOPT) -c $(COMMON_C) -o $(COMMON_O)

clean:
	rm -f $(OBJS)
