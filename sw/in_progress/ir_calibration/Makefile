
# Quiet compilation
Q=@


CC = gcc
CFLAGS=-g -O2 -Wall $(shell pkg-config gtk+-2.0 --cflags)
LDFLAGS=$(shell pkg-config gtk+-2.0 --libs) -lglibivy -lm -lgtkdatabox

ir_calib : main.c calibrator.c gui.c
	$(CC) $(CFLAGS) -g -o $@ $^ $(LDFLAGS)

clean:
	$(Q)rm -f *~ ir_calib
