CC=g++
INCFLAGS=
CFLAGS=-c -std=c++11 $(INCFLAGS)
LDFLAGS=

OBJECTS := $(wildcard *.cpp) $(wildcard *.c)

.PHONY = all $(PROGNAME) clean

all : $(PROGNAME)

$(PROGNAME) : $(OBJECTS)
	$(CC) -o $@ $^

%.o : %.cpp %.c %.h %.hpp
	$(CC) $(CFLAGS) -o $@ $<

clean :
	rm -rf *.o $(PROGNAME) 
