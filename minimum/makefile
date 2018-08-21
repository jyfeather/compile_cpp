main:clean start main.o stdafx.o hello.o
	#g++ main.o stdafx.o hello.o bye.o -o main
	g++ main.o stdafx.o hello.o ./dir/bye.o -o main
start:
	@cd ./dir; make; # @为关闭回声，不显示本行执行信息
main.o:main.cpp
	g++ -c main.cpp -o main.o
stdafx.o:stdafx.cpp stdafx.h
	g++ -Idir -c stdafx.cpp -o stdafx.o
hello.o:hello.cpp hello.h
	g++ -c hello.cpp -o hello.o
#bye.o:dir/bye.cpp dir/bye.h
#	g++ -c dir/bye.cpp -o bye.o
clean:
	rm -f *.o
