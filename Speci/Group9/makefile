CXX = g++
CXXFLAGS = -std=c++11 -g
H = Headers
HDRS = $(H)/Register.h $(H)/ProcessorStateWord.h $(H)/FpStatusWord.h\
$(H)/IntRegisterFile.h $(H)/FpRegisterFile.h $(H)/Memory.h\
$(H)/Cpu.h $(H)/Instruction.h $(H)/Group9.h

all: Group9.o Halt.o

Group9.o: Group9.C $(HDRS)
	gcc -c Group9.C -o Group9.o
Halt.o: Halt.C $(HDRS)
	gcc -c Halt.C -o Halt.o
clean:
	rm -f *.o
