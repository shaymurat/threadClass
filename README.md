# Домашнее задание по теме "Потоки на классах"

Если вы решали старую версию задачи, проверка будет производиться по ней.

Ссылка на старую версию [тут](https://docs.google.com/document/d/1gUPdl6CcPpZ_1XvItf3KMnBh0uxAUI9bnpvZLYHj-V4/edit?usp=sharing).

Цель: научиться создавать классы наследованные от класса ```Thread```.

## Задача "За честь и отвагу!":

Создайте класс ```Knight```, наследованный от ```Thread```, объекты которого
будут обладать следующими свойствами:
1. Атрибут ```name``` - имя рыцаря. (```str```)
2. Атрибут ```power``` - сила рыцаря. (```int```)

А также метод ```run```, в котором рыцарь будет сражаться с врагами:
1. При запуске потока должна выводится надпись "<Имя рыцаря>, на нас
   напали!".
2. Рыцарь сражается до тех пор, пока не повергнет всех врагов (у всех
   потоков их 100).
3. В процессе сражения количество врагов уменьшается на ```power``` текущего
   рыцаря.
4. По прошествию 1 дня сражения (1 секунды) выводится строка "<Имя
   рыцаря> сражается <кол-во дней>..., осталось <кол-во воинов>
   воинов."
5. После победы над всеми врагами выводится надпись "<Имя рыцаря>
   одержал победу спустя <кол-во дней> дней(дня)!"

Как можно заметить нужно сделать задержку в 1 секунду, инструменты для
задержки выберите сами.

Пункты задачи:
1. Создайте класс ```Knight``` с соответствующими описанию свойствами.
2. Создайте и запустите 2 потока на основе класса ```Knight```.
3. Выведите на экран строку об окончании битв.

Пример результата выполнения программы:

Алгоритм выполнения кода:
```
# Создание класса
first_knight = Knight('Sir Lancelot', 10)
second_knight = Knight("Sir Galahad", 20)
# Запуск потоков и остановка текущего
# Вывод строки об окончании сражения
```

Вывод на консоль:
```
Sir Lancelot, на нас напали!
Sir Lancelot, сражается 1 день(дня)..., осталось 90 воинов.
Sir Galahad, на нас напали!
Sir Galahad, сражается 1 день(дня)..., осталось 80 воинов.
Sir Galahad, сражается 2 день(дня)..., осталось 60 воинов.
Sir Lancelot, сражается 2 день(дня)..., осталось 80 воинов.
Sir Lancelot, сражается 3 день(дня)..., осталось 70 воинов.
Sir Galahad, сражается 3 день(дня)..., осталось 40 воинов.
Sir Lancelot, сражается 4 день(дня)..., осталось 60 воинов.
Sir Galahad, сражается 4 день(дня)..., осталось 20 воинов.
Sir Galahad, сражается 5 день(дня)..., осталось 0 воинов.
Sir Lancelot, сражается 5 день(дня)..., осталось 50 воинов.
Sir Lancelot, сражается 6 день(дня)..., осталось 40 воинов.
Sir Galahad одержал победу спустя 5 дней(дня)!
Sir Lancelot, сражается 7 день(дня)..., осталось 30 воинов.
Sir Lancelot, сражается 8 день(дня)..., осталось 20 воинов.
Sir Lancelot, сражается 9 день(дня)..., осталось 10 воинов.
Sir Lancelot, сражается 10 день(дня)..., осталось 0 воинов.
Sir Lancelot одержал победу спустя 10 дней(дня)!
Все битвы закончились!
```

Файл module_10_2.py и загрузите его на ваш GitHub репозиторий. В решении
пришлите ссылку на него.

Успехов!
