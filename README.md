
# func_zero_calc

## Описание

Эта программа предназначена для вычисления нулей функции на языке C в среде Linux.

## Установка (с помощью репозитория на GitHub)

1. Склонируйте репозиторий: git clone https://github.com/ada-dmitry/tmp_project.git
2. Перейдите в директорию проекта: cd /done_project
3. Следуйте указаниям пункта "Использование"

## Установка (с помощью архива .tar)

1. Распакуйте архив в любую удобную вам директорию.
2. С помощью терминала зайдите в распакованную директорию по заданному пути.
3. Следуйте указаниям пункта "Использование"

## Использование

0. Для нормальной работы программы необходимо установить программу GNU PLot и сборщик make
   (sudo apt install gnuplot || sudo apt install make)
1. Соберите программу: make
2. Запустите программу: make run
3. Строго следуйте указаниям программы, вводя границы отрезка, точность вычисления корня и
   выбирая метод вычисления.

## Замечания

0. В поля ввода границ и точности необходимо соблюдать несколько ограничений:
   а. Вводить числа(без использования иных символов, помимо знака отрицания в начале "-" или дробной точки ".")
   б. Не выходить за пределы типа double(1,7E–308 до 1,7E+308)
1. Для корректной работы программы, необходимо вводить отрезок, на котором есть лишь один корень
   (это можно проверить благодаря графику).
2. После вызова меню выбора действий (Ctrl+C) можно использовать как верхний регистр, так и нижний.
3. Не рекомендуется бесконечно вызывать Ctrl+C без выбора действия, это может повлечь ошибки
   вследствие переполнения памяти.

## Обработка сигнала SIGINT

    Программа обрабатывает сигнал SIGINT, что позволяет давать пользователю выбор действия

при нажатии сочетания клавиш Ctrl+C.

## Обработка сигнала SIGTSTP

    Программа обрабатывает сигнал SIGTSTP, переводящий программу в фоновый режим,

вновь предоставляя пользователю управлять терминалом, но возвращающий настройки терминала к исходным.

## Авторы

Антипенко Дмитрий Андреевич [C22-712]
Кузнецов Даниил Евгеньевич [C22-712]
Никитин Михаил Андреевич [C22-712]
Ускова Екатерина Александровна [C22-712]
