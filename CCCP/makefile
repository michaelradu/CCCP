CC = g++
MAIN = main

SOVIET = /home/paulk/Desktop/soviet-lfs-rebuild

OUTPUT = bin

FLAGS = -g -std=c++20 -pedantic


default:
	${CC} -c src/make.cpp ${FLAGS} -o ${OUTPUT}/make.o
	${CC} src/${MAIN}.cpp ${FLAGS} ${OUTPUT}/make.o  ${OUTPUT}/misc.o -o ${OUTPUT}/${MAIN}

run:
	./${OUTPUT}/${MAIN}
clean:
	rm -rf ${OUTPUT}
install:
	cp -r ${OUTPUT}/${MAIN} ${SOVIET}/bin/cccp
