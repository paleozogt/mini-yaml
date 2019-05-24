test: folders ../obj/test/test.o
	$(CXX) -o ../bin/test ../obj/test/test.o  -s  googletest/googletest/make/gtest_main.a -lpthread

../obj/test/test.o: test.cpp
	$(CXX) -std=c++11 -Igoogletest/googletest/include -I../yaml -c test.cpp -o ../obj/test/test.o

folders:
	mkdir -p ../bin
	mkdir -p ../obj/test
	

.PHONY: clean
clean:
	rm -r ../obj
