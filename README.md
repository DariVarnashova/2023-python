<h1> 2023-python <sup> co-made by <a href="https://github.com/Lyric-Meow/">Milly</a> </sup> </h1>
Лабораторные по курсу "Язык программирования Python", группы ИС-33, ИС-34

## Содержание:
- [Старт](#start)
- [Библиотеки](#libs)
- [Редакторы](#editors)
- [Полезное](#utility)
- [Предупреждения](#warnings)

- [1 Лабораторная](#lab1)
- [2 Лабораторная](#lab2)

<a name="start"></a>
## Старт:
- Для работы необходим python 3.9 и выше.

<a name="libs"></a>
### Библиотеки:

---

- numpy
- matplotlib
- tkinter

<a name="editors"></a>
### Редактор любой. Из неплохих:

---

- IDLE (родной, идёт вместе с установщиком)
- Visual Studio Code, notepad++
- PyCharm
- vim (для любителей сначала страдать, потом наслаждаться)

<a name="utility"></a>
## Полезное
<ul>
<Li>
Работа с блокнотами онлайн, с возможностью подключение удалённых мощностей гугла (GPU, TPU):
<a href="https://colab.research.google.com/">
<img src="https://img.shields.io/badge/Google%20Colab-2275be?logo=google&logoColor=fcec06" height="25" alt="Google colab Badge"/>
</a><br>
</Li>
<Li>
Презентация (будет обновляться в течение семестра): 
<a href="https://docs.google.com/presentation/d/1CqyrZYSh15dsVWt57eu14UDtm2-GFpSF5TD2_tVLaCc/edit?usp=sharing">
<img src="https://img.shields.io/badge/Google%20docs-2275be?logo=google&logoColor=fcec06" height="25" alt="Google Docs Badge"/>
</a><br>
</Li>
<Li>
Хорошая книга по python, очень простым языком и на понятных примерах: 
<a href="https://wombat.org.ua/AByteOfPython/AByteofPythonRussian-2.02.pdf">
<img src="https://img.shields.io/badge/Wombat-2275be?labelColor=fcec06" height="25" alt="Book Badge"/>
</a><br>
</Li>
<Li>
Сервер в Дискорд, где буду дублировать: 
<a href="https://discord.gg/MzPkCYf4Dh">
<img src="https://img.shields.io/badge/Discord-2275be?logo=discord&logoColor=fcec06" height="25" alt="Discord Badge"/>
</a><br>
</Li>
<Li>
Мой контакт:
<a href="mailto:nsmorozov@rf.unn.ru">
  <img src="https://img.shields.io/badge/E%E2%80%93mail-2275be?logo=gmail&logoColor=fcec06" height="25" alt="E–mail Badge"/>
</a>
</Ul>

<a name="warnings"></a>
## Предупреждения:
- В своей папке можете делать все что угодно, в чужие не залезать, в корневую тоже.
- Я буду ориентироваться на файлы, где в названии будет номер лабораторной.

<a name="lab1"></a>
## [1] Работа со структурами данных
	
### Исходные данные:

---

- свои ФИО, число, месяц, год рождения в виде кортежа;
- предметы в школьном аттестате (не меньше 14), как словарь из названия и оценки (можно мокать);
- имена (только) ближайших (до двоюродных включительно) родственников в списке;
- имя, которое вы бы дали своей домашней пушистой киве (строка).

### Действия:

---

<ol>
<Li> вывести среднюю оценку в аттестате;</Li>
<Li> вывести, исключив повторения, все различные имена среди своих родственников (включая свое);</Li>
<Li> общая длина всех названий предметов;</Li>
<Li> уникальные буквы в названиях предметов;</Li>
<Li> имя вашей домашней пушистой кивы в бинарном виде;</Li>
<Li> отсортированный по алфавиту (в обратном порядке) список родственников;</Li>
<Li> количество дней от вашей даты рождения до текущей даты (должна быть всегда актуальной);</Li>
<Li> FIFO очередь, в которую можно добавлять предметы по вводимому с клавиатуры индексу (до команды остановки), после введения - вывести все;</Li>
<Li> по введеному индексу, поменять имя в отсортированном списке родственников на имя ацтекского правителя (<a href="https://en.wikipedia.org/wiki/List_of_rulers_of_Tenochtitlan"><img src="https://img.shields.io/badge/Wikipedia-2275be?logo=Wikipedia&logoColor=fcec06" height="25" alt="Wiki Badge"/></a>) под номером, получаемым из вашей даты рождения: number = (day + month**2 + year) % 21 + 1;</Li>
<Li> создать связный список, как словарь, где ключ - имя родственника, а значение - индекс следующего имени по исходному списку (к этому моменту, отсортированному в обратном алфавитном порядке), упорядоченному по их (родственников) годам рождения (года или создать отдельным списком, или просто держите их в уме при составлении связного -- оба варианта валидны), исходный список при этом должен остаться неизменным </Li>
<Li> написать функцию-генератор (cвой вариант определяется как number = len("ФИО") * len (family_names) % 4):
<ol type="1" start="0">
<li> аликвотной последовательности; </li> 
<li> последовательности Сильвестра; </li> 
<li> числа трибоначчи;</li> 
<li> числа Леонардо. </li> 
</ol>
</Li>

</ol>

<a name="lab2"></a>
## [2] Алгоритмы сортировки

### Исходные данные:
	
---

- список целых чисел от 0 до 999999;
- список из 99999 случайных вещественных чисел в диапазоне [-1, 1];
- 42000 разных точки комплексной плоскости, лежащие на окружности радиуса r = birth_day / birth_month (можно случайных, можно равномерно распределённых);
- отрывок из книги (любой, на свой выбор) не менее 10000 слов, разбитый в список по словам.

### Действия:
	
---

Реализовать для каждого из исходных списков один из представленных алгоритмов сортировки (подробнее почитать о них [тут](https://habr.com/en/post/335920/)). Выбор тех четырех алгоритмов, которые будут использованы конкретно у вас: 

>import random

>random.sample(range(1, 18), 4) # вернет список из 4 случайных значений в заданном диапазоне, сделать один раз

1. shaker sort, сортировка перемешиванием;
2. bubble sort, сортировка пузырьком;
3. comp sort, сортировка расческой;
4. insertion sort, сортировка вставкой;
5. Shellsort, сортировка Шелла;
6. tree sort, сортировка деревом;
7. Gnome sort, гномья сортировка;
8. selection sort, сортировка выбором;
9. Heapsort, пирамидальная сортировка;
10. Quicksort, быстрая сортировка;
11. Merge sort, сортировка слиянием;
12. Counting sort, сортировка подсчетом;
13. Bucket sort, блочная (карманная) сортировка;
14. Radix sort, поразрядная сортировка;
15. least significant digit;
16. most significant digit;
17. bitonic sort, битонная сортировка;
18. timsort, гибридная сортировка.
