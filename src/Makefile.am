bin_PROGRAMS = ssw_test example_c example_cpp

pkginclude_HEADERS = ssw.h ssw_cpp.h
lib_LTLIBRARIES = libssw.la
libssw_la_SOURCES = ssw.c ssw.h ssw_cpp.h ssw_cpp.cpp
libssw_la_LDFLAGS = -version-info 0:0:0

LDADD = libssw.la

ssw_test_SOURCES = main.c kseq.h

example_c_SOURCES = example.c
example_c_LDADD = $(LDADD) -lm -lz

example_cpp_SOURCES = example_cpp.cpp
example_cpp_LDADD = $(LDADD) -lm -lz

# we are not making java related staff

#JAVA_JAR = ssw.jar
#JAVA_LIB = libsswjni.so
#JAVA_INLCUDES = -I"$(JAVA_HOME)/include" -I"$(JAVA_HOME)/include/linux"
#JAVA_OBJ = ssw/Aligner.class ssw/Alignment.class ssw/Example.class

#all: default java

#java: $(JAVA_JAR) $(JAVA_LIB)

#$(JAVA_LIB): sswjni.c ssw.c ssw.h
#	$(CC) $(CFLAGS) $(JAVA_INLCUDES) -fPIC -shared -rdynamic -o $@ $< ssw.c 

#$(JAVA_JAR): $(JAVA_OBJ)
#	jar cvfe $@ ssw.Example $^

