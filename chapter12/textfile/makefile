textfile: textfile.o linlib.o
	gcc -m32 textfile.o linlib.o -o textfile
textfile.o: textfile.asm
	nasm -f elf -g -F stabs textfile.asm
linlib.o: linlib.asm
	nasm -f elf -g -F stabs linlib.asm
clean:
	rm *.lst
	rm *.o
	rm textfile
run: textfile
	./textfile
