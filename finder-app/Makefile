
CC := $(CROSS_COMPILE)gcc
CFLAGS := -Wall -Wextra -O2
TARGET := writer
SRC := writer.c
OBJ := $(SRC:.c=.o)


all: $(TARGET)


$(TARGET): $(OBJ)
	$(CC) $(CFLAGS) -o $@ $^


%.o: %.c
	$(CC) $(CFLAGS) -c $< -o $@


clean:
	rm -f $(TARGET) *.o

