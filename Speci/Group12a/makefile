
CXX=g++
CXXFLAGS= -std=c++11 -g
H = Headers
HDRS = $(H)/Register.h $(H)/ProcessorStateWord.h $(H)/FpStatusWord.h\
$(H)/IntRegisterFile.h $(H)/FpRegisterFile.h $(H)/Memory.h\
$(H)/Cpu.h $(H)/Instruction.h $(H)/Group12a.h

all: Group12a.o Trap.o

Group12a.o: Group12a.C $(HDRS)
	gcc -c Group12a.C -o Group12a.o

Trap.o: Trap.C $(HDRS)
	gcc -c Trap.C -o Trap.o


clean: 
	rm -f *.o

