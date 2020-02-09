all: add_server add_client

add_server: add_server.o add_svc.o add_xdr.o
		gcc -o add_server add_server.o add_svc.o add_xdr.o
add_client: add_client.o add_clnt.o add_xdr.o
		gcc -o add_client add_client.o add_clnt.o add_xdr.o
add_server.o: add_server.c add.h
		gcc -c add_server.c
add_svc.o: add_svc.c add.h
		gcc -c add_svc.c
add_client.o: add_client.c add.h
		gcc -c add_client.c
add_clnt.o: add_clnt.c add.h
		gcc -c add_clnt.c
add_xdr.o: add_xdr.c add.h
		gcc -c add_xdr.c
clean:
		rm add_server add_client *.o
