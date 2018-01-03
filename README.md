# Tcp-Client-Server-using-C

A virtual project to develop a connection between server and client using TCP connection in C language in UNIX platform. Here server acts a concurrent server, where single server virtually can handle multiple clients at a time.


/*Devineni, Sai Dheeraj --- devinenis7463@uhcl.edu ----- ID:1595002-------*/

Compilation Of The Program At Server Side :
-------------------------------------------
First should give 'gcc' '-g' '-o' 'output name' 'filename' '-lnsl' 'lsocket' 'lresolv'(Last three commands for linking purpose) and then enter

Example
-------
gcc -g -o serv DevineniTcpServer.c -lnsl -lsocket -lresolv

Execution Of The Program :
------------------------
1)Need to give command ./serv port_number and then enter.
2)After that it will accept the request from client side and receive the commands from client side and execute it and prints the output at client side.

Example
-------
./serv 15002

Compilation Of The Program At Client Side :
-------------------------------------------
First should give 'gcc' 'filename' '-lnsl' 'lsocket' 'lresolv'(Last three commands for linking purpose) and then enter

Example
-------
gcc  DevineniTcpClient.c -lnsl -lsocket -lresolv

Execution Of The Program :
------------------------
1)Need to give command ./serv ip_address port_number and then enter.
2)After that it will ask to enter the commands, so please enter the commands u want to execute with spaces only in between commands, otherwise it will not work.
3)It sends the coomands to server.
4)It receives the output of the commands from the server and prints it.
5)After completion it will ask to quit--->press 'q' or else press any other character to continue.

Example
-------
./a.out 10.0.0.9 15002

Dheeraj--->Enter the commands:ls -l | sort | wc (Have spaces in between)

Enter q to quit or enter any other letter to continue ('q' to quit or else other key to continue)
