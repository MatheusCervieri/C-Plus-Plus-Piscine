NAME		=	ex01
CC			=	c++
INCLUDES	=	includes
CPPFLAGS	=	-Wall -Werror -Wextra -std=c++98 
RM			=	rm -rf
SRCS		=	main.cpp \
				Dog.cpp \
				Animal.cpp \
				Cat.cpp \
				Brain.cpp

OBJS		=	$(SRCS:%.cpp=%.o)

all:		$(NAME)

$(NAME):	$(OBJS)
			@$(CC) $(CPPFLAGS) $(OBJS) -o $(NAME)

.cpp.o:
			@$(CC) $(CPPFLAGS) -c $< -o $(<:.cpp=.o)

clean:
			@$(RM) $(OBJS)

fclean:		clean
			@$(RM) $(NAME)

re:			fclean all

.PHONY:		fclean, all, re