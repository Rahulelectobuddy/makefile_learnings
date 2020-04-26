#get cacu bin file
example2:add_int.o add_float.o sub_int.o sub_float.o main.o
	gcc -o example add/add_int.o add/add_float.o \
		sub/sub_int.o sub/sub_float.o main.o -ggdb

#get add_int.o target
add_int.o:
	gcc -o add/add_int.o -c add/add_int.c -ggdb

#get add_float.o target
add_float.o:
	gcc -o add/add_float.o -c add/add_float.c -ggdb

#get sub_int.o target
sub_int.o:
	gcc -o sub/sub_int.o -c sub/sub_int.c -ggdb

#get sub_float.o target
sub_float.o:
	gcc -o sub/sub_float.o -c sub/sub_float.c -ggdb

#get main.o target
main.o:
	gcc -o main.o -c main.c -Iadd -Isub -ggdb

#clean project
clean:
	rm -f example add/add_int.o add/add_float.o \
		sub/sub_int.o sub/sub_float.o main.o
