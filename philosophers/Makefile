# **************************************************************************** #
#                                                                              #
#                                                         :::      ::::::::    #
#    Makefile                                           :+:      :+:    :+:    #
#                                                     +:+ +:+         +:+      #
#    By: jmacera- <jmacera-@student.42.fr>          +#+  +:+       +#+         #
#                                                 +#+#+#+#+#+   +#+            #
#    Created: 2024/05/16 13:34:35 by jmacera-          #+#    #+#              #
#    Updated: 2024/05/16 13:41:32 by jmacera-         ###   ########.fr        #
#                                                                              #
# **************************************************************************** #

NAME	= philo

HEADER	= ./include/

CC		= gcc

CFLAGS	= -Werror -Wall -Wextra -g -I $(HEADER) -pthread

SRCS	= srcs/main.c \
			srcs/activity.c \
			srcs/threads.c \
			srcs/init_and_parse.c \
			srcs/utils_philo.c \
			srcs/utils_lib.c \

OBJS	= $(SRCS:.c=.o)

all		: $(NAME)

$(NAME)	: $(OBJS) $(HEADER)
			$(CC) $(FLAGS) $(OBJS) -o $(NAME)

clean	: rm -rf $(OBJS)

fclean	: clean
			rm -rf $(NAME)

re		: fclean all
