# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: mvieira- <mvieira-@student.42sp.org.br>    +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/10/11 12:06:36 by mvieira-          #+#    #+#              #
#    Updated: 2022/10/11 12:23:31 by mvieira-         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME		=	Zombie
CC			=	c++
INCLUDES	=	includes
CPPFLAGS	=	-Wall -Werror -Wextra -std=c++98 -I$(INCLUDES)
RM			=	rm -rf

SRCS		=	Zombie.class.cpp \
				main.cpp \
				randomChump.cpp \
				newZombie.cpp

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