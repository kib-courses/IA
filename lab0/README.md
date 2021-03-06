# Домашняя работа №0

Домашняя работа сдаётся на собеседовании после второй лекции и влияет на поступление на спецкурс

Дата сдачи: до 29 октября 2020

## Задание

Реализовать на языке С/С++ функцию копирования памяти, 
которая имеет следующий [прототип](https://ru.wikipedia.org/wiki/Прототип_функции):

## Срок сдачи

  
```C
errno_t my_memcpy_s(void *restrict dest, rsize_t destsz, const void *restrict src, rsize_t count ).
```

  * Сравнить скорость работы my_memcpy_s с функцией memcpy_s из стандартной библиотеки С/С++, вычислив среднее время работы обеих функции на следующих объемах данных: 
     1. 16 байт, 
     1. 700 байт, 
     1. 16 Кбайт, 
     1. 4Мбайта 
  * Количество повторений для каждого теста из п.1 **N=100**. Посчитать [среднее](https://ru.wikipedia.org/wiki/Математическое_ожидание).
  * В качестве компиляторов для С/С++ использовать **GCC**, **Clang** или **ICC** (Intel C/C++ Compiler)
  * Можно использовать ассемблерные вставки или отдельные ассемблерные модули. 
  * Замеры проводить для 32-х битного и 64-х битного кода. 
  
  * При компиляции использовать оптимизацию. Например, для **GCC/ICC** нужно использовать следующие параметры:  
 ```
 -O2 -march=native -funroll-loops. 
 ```
  
  * **Требование:** реализованная функция должна работать не более чем на 15% медленнее в каждом тесте.  
  * **Усложнение 1:** При проведении тестов использовать функцию _intel_fast_memcpy для сравнения с собственной реализацией.  
  * **Усложнение 2:** Ваша функция должна работать не хуже, чем _intel_fast_memcpy. 
  * ** Анализ производительности можно проводить при помощи [Intel VTune Performance Analyzer](https://en.wikipedia.org/wiki/VTune) / [Perf](https://en.wikipedia.org/wiki/Perf_(Linux))