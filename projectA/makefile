main:main.c lib/libcal.a
	gcc main.c -o main -lcal -Llib -I include
lib/libcal.a:lib/add.o lib/sub.o
	ar rcs lib/libcal.a lib/add.o lib/sub.o
lib/add.o:src/add.c
	gcc -I include -c src/add.c -o lib/add.o
lib/sub.o:src/sub.c
	gcc -I include -c src/sub.c -o lib/sub.o
.PHONY:clean
clean:
	rm lib/*.o
	rm main	
