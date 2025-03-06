# 📌 Critical Path Calculator (Калькулятор критического пути)
### 📖 Описание
Эта программа реализует метод критического пути (CPM) для рассчета и анализа задач проекта. Она рассчитывает:

Раннее начало (ES) и окончание (EF) для каждой работы.
Позднее начало (LS) и окончание (LF).
Запас времени (Slack).
Критический путь, определяющий минимальное время завершения проекта.
### Установка и запуск
1. Cкачайте как zip файл и распакуйте
2. Запустите .exe файл

### ⌨️ Синтаксис ввода
Каждая работа вводится в формате:

<Номер работы>,<Предшественники>,<Время работы>

###### 📌 Синтаксис:
```
1,,3 → Работа 1, без предшественников, длится 3 единицы времени.2,1,5 → Работа 2 зависит от 1-й, длится 5 единиц времени.
4,2;3,4 → Работа 4 зависит от 2-й и 3-й, длится 4 единицы времени.
👉 Для завершения ввода введите 0.
```
###### 📊 Пример работы
###### Условие
| Номер задачи | Предшественники | Время |
| ------------ | --------------- | ----- |
| 1            | -               | 3     |
| 2            | -               | 5     |
| 3            | 2               | 1     |
| 4            | 1, 3            | 2     |
###### Ввод
'''
Введите данные работы: 1,,3
Введите данные работы: 2,,5
Введите данные работы: 3,2,1
Введите данные работы: 4,1;3,2
Введите данные работы: 0
'''
###### Вывод
'''
Параметры работ:Работа   ES   EF   LS   LF  Запас  Критическая
     1    0    3    3    6      3          Нет
     2    0    5    0    5      0           Да
     3    5    6    5    6      0           Да
     4    6    8    6    8      0           Да

Общее время выполнения проекта: 8

Критический путь (последовательность работ):
2 -> 3 -> 4
'''

📜 Лицензия
Этот проект распространяется под лицензией MIT.
👤 Автор
medoed687 - https://github.com/medoed687
