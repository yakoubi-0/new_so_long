# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: ayakoubi <ayakoubi@student.1337.ma>        +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2022/10/18 17:34:53 by ayakoubi          #+#    #+#              #
#    Updated: 2023/02/12 12:47:22 by ayakoubi         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	=	libftprintf.a
SRC		=	ft_printf.c \
			ft_putchar.c \
			ft_putnbr.c \
			ft_putstr.c \
			ft_putuns.c \
			ft_puthex.c

OBJ		=	$(SRC:.c=.o)

CC		=	cc

CFLAGS	=	-Wall -Wextra -Werror

all	:	$(NAME)

%.o:%.c
	@$(CC) $(CFLAGS) -c $< -o $@

$(NAME)	:	$(OBJ)
	@ar -rcs $@ $^

clean	:
	@rm -f *.o

fclean	:	clean
	@rm -f *.a

re : fclean all

.PHONY : all clean fclean re

