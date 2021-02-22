Sort: sort.o bubbleSort.o mergeSort.o quickSort.o
	gcc sort.o bubbleSort.o mergeSort.o quickSort.o -o Sort

bubbleSort.o: bubbleSort.c bubbleSort.h
	gcc -c -g  bubbleSort.c -o bubbleSort.o

mergeSort.o: mergeSort.c mergeSort.h
	gcc -c -g mergeSort.c -o mergeSort.o

quickSort.o: quickSort.c quickSort.h
	gcc -c -g quickSort.c -o quickSort.o

sort.o: sort.c bubbleSort.h mergeSort.h quickSort.h types.h
	gcc -c -g sort.c -o sort.o

clean:
	rm -f *.o
