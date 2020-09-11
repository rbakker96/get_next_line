Get Next Line - Reading a line on a fd is way too tedious

--------------------- Project summary ---------------------

This project will not only allow you to add a very convenient function to your collection, but it will also allow you to learn a highly interesting new concept in C programming: static variables.

--------------------- Technical considerations ---------------------

• Calling your function get_next_line in a loop will then allow you to read the text available on a file descriptor one line at a time until the EOF.

• Make sure that your function behaves well when it reads from a file and when it reads from the standard input.

• libft is not allowed for this project. You must add a get_next_line_utils.c file which will contain the functions that are needed for your get_next_line to work.

• Your program must compile with the flag -D BUFFER_SIZE=xx. which will be used as the buffer size for the read calls in your get_next_line. This value will be modified by your evaluators and by moulinette.

• Compilation will be done this way : gcc -Wall -Wextra -Werror -D BUFFER_SIZE=32 get_next_line.c get_next_line_utils.c

• Your read must use the BUFFER_SIZE defined during compilation to read from a file or from stdin.

• In the header file get_next_line.h you must have at least the prototype of the function get_next_line.

• We consider that get_next_line has an undefined behavior if, between two calls, the same file descriptor switches to a different file before EOF has been reached on the first fd.

• lseek is not an allowed function. File reading must be done only once.

• Finally we consider that get_next_line has an undefined behavior when reading from a binary file. However, if you wish, you can make this behavior coherent.

• Global variables are forbidden.

--------------------- Used resources ---------------------

Most important new concepts which I needed to master and important resources used with that.

• File Descripter / open / read -
https://www.geeksforgeeks.org/input-output-system-calls-c-create-open-close-read-write/

• Static Variables in C - 
https://www.geeksforgeeks.org/static-variables-in-c/
