eatsyscall: eatsyscall.o
	ld -m elf_i386 -o eatsyscall eatsyscall.o
eatsyscall.o: eatsyscall.asm
	nasm -f elf -g -F stabs eatsyscall.asm -l eatsyscall.lst
clean:
	rm *.lst
	rm *.o
	rm eatsyscall
run: eatsyscall
	./eatsyscall
