A simple client and server program. The server is executing on its host machine a subset
of Unix commands.

The commands that are allowed are the following:

ls, cat,cut, grep and tr

myserver.c


1)void clean_up_child_process (int);
2)void timeToStop();
3)int read_from_client (int,struct hostent* );
4)main();

myclient.c


1)void myhandler()--handler--
2)void sigpipehandler()--handler--
3)main(int argc, char *argv[])