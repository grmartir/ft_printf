NAME = libftprintf.a
SRC = $(shell find . -name '*.c')
OBJ = $(SRC:.c=.o)
CC = cc
FLAGS = -Wall -Werror -Wextra
AR = ar r
RM = rm -f

all : $(NAME)

%.o : %.c 
	$(CC) $(FLAGS) -c $< -o $@

$(NAME) : $(OBJ)
	$(AR) $(NAME) $(OBJ)

fclean		: clean
	$(RM)  $(NAME)

clean :
	$(RM) $(OBJ)

re: fclean all

.PHONY : all, clean, fclean, bonus, re
