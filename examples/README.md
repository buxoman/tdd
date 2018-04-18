# To build the examples

## Command Line:

for gcc:
make clean all test gcov

## CodeLite IDE

Modify project's setting:

Compiler:

include path:  .;../../../cpputest/include

Linker:

Libraries:  CppUTest;CppUTestExt;

Build:

make -C $(WorkspacePath)/examples -f Makefile clean all test gcov

Clean:

make -C $(WorkspacePath)/examples -f Makefile clean