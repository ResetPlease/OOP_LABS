# Отчёт по лабораторной работе №1 по курсу "Объектно-ориентированное программирование"

## 1. Тема

Первая программа на C++

## 2. Цель работы

- Изучить систему сборки CMake
- Изучить базовые операторы и конструкции C++
- Изучить библиотеку для написания Unit-тестов Google Test
- Научится писать простые программы, использующие ввод/вывод через потоки std::cin и std::cout

## 3. Задание (вариант № 3)

Напишите функцию, которая принимает строку круглых скобок и определяет, является ли порядок скобок правильным. Функция должна возвращать true, если строка допустима, и false, если недопустима.
Все входные данные будут строками, состоящими только из символов ( и ).
Пустые строки считаются сбалансированными (и, следовательно, валидными) и будут проверяться.

## 4. Тестирование

```bash
╭─ ~/codes/MAI/OOP/OOP_labs/lab1/build
╰─❯ cmake .. && make && ./tests
-- The C compiler identification is GNU 9.4.0
-- The CXX compiler identification is GNU 9.4.0
-- Check for working C compiler: /usr/bin/cc
-- Check for working C compiler: /usr/bin/cc -- works
-- Detecting C compiler ABI info
-- Detecting C compiler ABI info - done
-- Detecting C compile features
-- Detecting C compile features - done
-- Check for working CXX compiler: /usr/bin/c++
-- Check for working CXX compiler: /usr/bin/c++ -- works
-- Detecting CXX compiler ABI info
-- Detecting CXX compiler ABI info - done
-- Detecting CXX compile features
-- Detecting CXX compile features - done
-- Found GTest: /home/beregom/anaconda3/lib/cmake/GTest/GTestConfig.cmake (found version "1.10.0")  
-- Configuring done
-- Generating done
-- Build files have been written to: /home/beregom/codes/MAI/OOP/OOP_labs/lab1/build
Scanning dependencies of target tests
[ 16%] Building CXX object CMakeFiles/tests.dir/tests.cpp.o
[ 33%] Building CXX object CMakeFiles/tests.dir/solve.cpp.o
[ 50%] Linking CXX executable tests
[ 50%] Built target tests
Scanning dependencies of target task
[ 66%] Building CXX object CMakeFiles/task.dir/main.cpp.o
[ 83%] Building CXX object CMakeFiles/task.dir/solve.cpp.o
[100%] Linking CXX executable task
[100%] Built target task
[==========] Running 7 tests from 7 test suites.
[----------] Global test environment set-up.
[----------] 1 test from test1
[ RUN      ] test1.brackets
[       OK ] test1.brackets (0 ms)
[----------] 1 test from test1 (0 ms total)

[----------] 1 test from test2
[ RUN      ] test2.brackets
[       OK ] test2.brackets (0 ms)
[----------] 1 test from test2 (0 ms total)

[----------] 1 test from test3
[ RUN      ] test3.brackets
[       OK ] test3.brackets (0 ms)
[----------] 1 test from test3 (0 ms total)

[----------] 1 test from test4
[ RUN      ] test4.brackets
[       OK ] test4.brackets (0 ms)
[----------] 1 test from test4 (0 ms total)

[----------] 1 test from test5
[ RUN      ] test5.brackets
[       OK ] test5.brackets (0 ms)
[----------] 1 test from test5 (0 ms total)

[----------] 1 test from test6
[ RUN      ] test6.brackets
[       OK ] test6.brackets (0 ms)
[----------] 1 test from test6 (0 ms total)

[----------] 1 test from test7
[ RUN      ] test7.brackets
[       OK ] test7.brackets (0 ms)
[----------] 1 test from test7 (0 ms total)

[----------] Global test environment tear-down
[==========] 7 tests from 7 test suites ran. (0 ms total)
[  PASSED  ] 7 tests.
```
