
# TDD - Calculadora

Este é o código exemplo do trabalho usando TDD (*Test Driven Development*) com o framework C++ [Catch2](https://github.com/catchorg/Catch2/tree/v2.x).


O framework Catch2 consegue ser utilizado apenas com o arquivo header [catch.hpp](catch.hpp) sem necessidade de instalação.

**NÃO MODIFIQUE OS TESTES** 

Todos os testes estão prontos no arquivo [calculadora.cpp](calculadora.cpp). A compilação e teste pode ser feita com os comandos:
```
$ g++ -Wall -std=c++11 -o calc calculadora.cpp 
```

A saída resumida do teste (código exemplo):
```
$ ./calc --reporter compact --success
calculadora.cpp:72: passed: c.fim() == false for: false == false
calculadora.cpp:81: passed: c.fim() == true for: true == true
calculadora.cpp:82: passed: c.resultado() == 1 for: 1 == 1
calculadora.cpp:91: failed: c.fim() == false for: true == false
calculadora.cpp:100: failed: c.fim() == false for: true == false
calculadora.cpp:108: passed: c.fim() == false for: false == false
calculadora.cpp:116: failed: c.fim() == true for: false == true
calculadora.cpp:125: failed: c.fim() == true for: false == true
calculadora.cpp:134: failed: c.fim() == true for: false == true
calculadora.cpp:143: failed: c.fim() == true for: false == true
calculadora.cpp:152: failed: c.fim() == true for: false == true
calculadora.cpp:161: failed: c.fim() == true for: false == true
calculadora.cpp:170: failed: c.fim() == true for: false == true
calculadora.cpp:179: failed: c.fim() == true for: false == true
calculadora.cpp:188: passed: c.fim() == false for: false == false
calculadora.cpp:196: passed: c.fim() == false for: false == false
calculadora.cpp:203: failed: c.fim() == true for: false == true
calculadora.cpp:212: failed: c.fim() == true for: false == true
calculadora.cpp:220: failed: c.fim() == true for: false == true
Failed 13 test cases, failed 13 assertions.
```

A saída completa do teste (código exemplo):
```
$ ./calc

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
a.out is a Catch v2.13.3 host application.
Run with -? for options

-------------------------------------------------------------------------------
1 2
-------------------------------------------------------------------------------
calculadora.cpp:86
...............................................................................

calculadora.cpp:91: FAILED:
  REQUIRE( c.fim() == false )
with expansion:
  true == false

-------------------------------------------------------------------------------
1+ = erro
-------------------------------------------------------------------------------
calculadora.cpp:95
...............................................................................

calculadora.cpp:100: FAILED:
  REQUIRE( c.fim() == false )
with expansion:
  true == false

-------------------------------------------------------------------------------
3+2+9 = 14
-------------------------------------------------------------------------------
calculadora.cpp:112
...............................................................................

calculadora.cpp:116: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
-1+3-5 = -3
-------------------------------------------------------------------------------
calculadora.cpp:121
...............................................................................

calculadora.cpp:125: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
30-15+8 = 23
-------------------------------------------------------------------------------
calculadora.cpp:130
...............................................................................

calculadora.cpp:134: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
3*8+7 = 31
-------------------------------------------------------------------------------
calculadora.cpp:139
...............................................................................

calculadora.cpp:143: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
3*7+4/3 = 22
-------------------------------------------------------------------------------
calculadora.cpp:148
...............................................................................

calculadora.cpp:152: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
(3+4)*2+7 = 21
-------------------------------------------------------------------------------
calculadora.cpp:157
...............................................................................

calculadora.cpp:161: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
3+4*(9+3) = 51
-------------------------------------------------------------------------------
calculadora.cpp:166
...............................................................................

calculadora.cpp:170: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
(3+1)*(4+7)+3-1 = 46
-------------------------------------------------------------------------------
calculadora.cpp:175
...............................................................................

calculadora.cpp:179: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
3.1+5.7-3.3 = 5.5
-------------------------------------------------------------------------------
calculadora.cpp:199
...............................................................................

calculadora.cpp:203: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
7/4+1 = 2.75
-------------------------------------------------------------------------------
calculadora.cpp:208
...............................................................................

calculadora.cpp:212: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

-------------------------------------------------------------------------------
3.3*2+7.796 = 14.396
-------------------------------------------------------------------------------
calculadora.cpp:216
...............................................................................

calculadora.cpp:220: FAILED:
  REQUIRE( c.fim() == true )
with expansion:
  false == true

===============================================================================
test cases: 18 | 5 passed | 13 failed
assertions: 19 | 6 passed | 13 failed

```

