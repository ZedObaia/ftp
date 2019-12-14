CC := gcc
CFLAGS := -Wall -g -Os

SHDIR := ../common

OBJS = ftclient.o $(SHDIR)/common.o

all: ftclient

ftclient: $(OBJS)
	@$(CC) -o ftclient $(CFLAGS) $(OBJS)

$(OBJS) : %.o: %.c 
	@$(CC) -c $(CFLAGS) $< -o $@

.PHONY:
clean:
	@rm -f *.o ftclient
	@rm -f ../common/*.o
	@rm -f server.txt
	@echo Done cleaning
