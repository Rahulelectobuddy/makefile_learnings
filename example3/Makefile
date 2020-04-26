CC = gcc
CFLAGS = -Iadd -Isub -O2
OBJDIR = objs
VPATH = add:sub:.
OBJS = add_int.o add_float.o sub_int.o sub_float.o main.o
TARGET = example3
RM = rm -f

$(TARGET):$(OBJDIR) $(OBJS)
	$(CC) -o $(TARGET) $(OBJDIR)/*.o $(CFLAGS)

$(OBJDIR):
	mkdir -p ./$@

$(OBJS):%.o:%.c
	$(CC) -c $(CFLAGS) $< -o $(OBJDIR)/$@

clean:
	-$(RM) $(TARGET)
	-$(RM) $(OBJDIR)/*.o -r
