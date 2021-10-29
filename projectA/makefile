main-v1:main.c lib/libcal.a
	gcc $< -o $@ -lcal -Llib -I include
lib/libcal.a:lib/add.o lib/sub.o
	ar rcs $@ $^
lib/add.o:src/add.c
	gcc -I include -c $< -o $@
lib/sub.o:src/sub.c
	gcc -I include -c $< -o $@
.PHONY:clean
clean:
	rm lib/*.o
	rm main-v1	
