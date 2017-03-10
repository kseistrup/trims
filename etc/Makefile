# KISS Makefile to merge a number of sources into a services file

SERVICES = services.pacnew services.local

all: services

services: $(SERVICES)
	trims -o $@ $(SERVICES)

.PHONY: clean

clean:
	@rm -vf *~

# eof
