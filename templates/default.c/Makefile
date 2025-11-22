flags= -O2 -Wall -std=c2x
# ldflags= -lbu

.PHONY: all clean

all: PROJECTNAME clean 

PROJECTNAME: PROJECTNAME.o
	@echo "Building..."
	@gcc $(flags) $^ -o $@ $(ldflags)

PROJECTNAME.o: PROJECTNAME.c PROJECTNAME.h
	@gcc $(flags) -c $<

clean:
	@echo "Cleaning..."
	@rm -f *.o