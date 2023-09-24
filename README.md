В этом репозитории предложены задания для курса по вычислениям на видеокартах 2023

[Остальные задания](https://github.com/GPGPUCourse/GPGPUTasks2023/).

# Задание 4. Транспонирование матрицы, умножение матриц.

[![Build Status](https://github.com/GPGPUCourse/GPGPUTasks2023/actions/workflows/cmake.yml/badge.svg?branch=task04&event=push)](https://github.com/GPGPUCourse/GPGPUTasks2023/actions/workflows/cmake.yml)

0. Сделать fork проекта
1. Выполнить задания 4.1 и 4.2 ниже
2. Отправить **Pull-request** с названием```Task04 <Имя> <Фамилия> <Аффиляция>``` (добавив в описании вывод работы программы в **pre**-тэгах - см. [пример](https://raw.githubusercontent.com/GPGPUCourse/GPGPUTasks2023/task04/.github/pull_request_example.md))

**Дедлайн**: 23:59 1 октября.

Задание 4.1. Транспонирование матрицы
=========

Реализуйте транспонирование матрицы таким образом, чтобы доступ и на чтение и на запись к глобальной видеопамяти был coalesced. (т.е. через локальную память)

Файлы: ```src/main_matrix_transpose.cpp``` и ```src/cl/matrix_transpose.cl```

Задание 4.2. Умножение матриц
=========

4.2.0 Реализуйте наивное умножение матриц через глобальную память

4.2.1 Реализуйте умножение матриц через локальную память. (на лекции это вплоть до "Умножение матриц 2: локальная память")

4.2.2 Реализайте умножение матриц через локальную память с большим количеством работы на один воркайтем (на лекции на странице "Умножение матриц 3: more work per thread". На странице с дожиманиями перемножения матриц это [кернел №3](https://cnugteren.github.io/tutorial/pages/page5.html))

4.2.3 Сравните производительность трех реализаций


Файлы: ```src/main_matrix_multiplication.cpp``` и ```src/cl/matrix_multiplication.cl```
