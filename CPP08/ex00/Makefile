CC = c++
CFLAGS = -Werror -Wall -Wextra -std=c++98
SRC = main.cpp
OBJ = $(SRC:.cpp=.o)
NAME = exec

all: $(NAME)

$(NAME): $(OBJ)
	$(CC) -o $(NAME) $(OBJ)

%.o: %.cpp
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ)

fclean: clean
	rm -f $(NAME)

re: fclean all