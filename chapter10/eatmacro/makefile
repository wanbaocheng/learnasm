eatmacro: eatmacro.o
	ld -m elf_i386 -o eatmacro eatmacro.o
eatmacro.o: eatmacro.asm
	nasm -f elf -l eatmacro.lst -g -F stabs eatmacro.asm
clean:
	rm *.lst
	rm *.o
	rm eatmacro
run: eatmacro
	./eatmacro
