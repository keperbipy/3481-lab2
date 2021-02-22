
CC = g++
H = Headers
HDRS = $(H)/Register.h $(H)/ProcessorStateWord.h $(H)FpStatusWord.h\
$(H)/IntRegisterFile.h $(H)/FpRegisterFile.h $(H)/Memory.h\
$(H)/Cpu.h $(H)/Instruction.h

OBJS = speci.o Register.o ProcessorStateWord.o FpStatusWord.o\
IntRegisterFile.o FpRegisterFile.o Memory.o Cpu.o Loader.o

build:
	(cd Group12a; make)
	(cd Group9; make)
	make speci

speci: $(OBJS)
	gcc $(OBJS) -o speci

Register.o: Register.C 
	gcc -c Register.C -o Register.o

ProcessorStateWord.o: ProcessorStateWord.C 
	gcc -c ProcessorStateWord.C -o ProcessorStateWord.o

FpStatusWord.o: FpStatusWord.C 
	gcc -c FpStatusWord.C -o FpStatusWord.o

IntRegisterFile.o: IntRegisterFile.C 
	gcc -c IntRegisterFile.C -o IntRegisterFile.o

FpRegisterFile.o: FpRegisterFile.C 
	gcc -c FpRegisterFile.C -o FpRegisterFile.o

Memory.o: Memory.C 
	gcc -c Memory.C -o Memory.o

Cpu.o: Cpu.C 
	gcc -c Cpu.C -o Cpu.o

Instruction.o: Instruction.C
	gcc -c Instruction.C -o Instruction.o 

Loader.o: Loader.C 
	gcc -c Loader.C -o Loader.o

speci.o: speci.C
	gcc -c speci.C -o speci.o




clean:
	rm -f *.o
	(cd Group12a; make clean)
	(cd Group9; make clean)
