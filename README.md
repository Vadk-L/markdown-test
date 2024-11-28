# markdown-test### Задание 1.1
```python
class Test:
    version = 1

a = Test()
a.version = 22
```

Будет ли изменен `Test.version` после выполнения этого кода?

##### Варианты ответа:
0) Да, так как он является ссылкой на объект класса
1) Нет, так как мы обновляем значение внутри пространства имен экземпляра
Ваш ответ: 1

---

### Задание 1.2
```python
class Test:
    version = 1

a = Test()
Test.version = 22
print(a.version)
```

Какое значение получим на выходе?

##### Варианты ответа:
0) 1, так как значение экземпляра сохраняется отдельно от класса
1) 22, так как мы изменили значение используя адрес в памяти, на который ссылаются экземпляры
Ваш ответ: 1

---

### Задание 1.3
Чем отличается экземпляр от класса?

##### Варианты ответа:
0) Класс создается из экземпляра
1) Экземпляр создается из класса
2) Ничем
Ваш ответ: 1

---

### Задание 1.4
Напишите класс, который будет содержать атрибут `version`, значение которого 100. После чего используя `getattr` необходимо получить атрибут `version` и вывести его на экран.

##### Ваша реализация кода:
```python
class Test:
    pass

```

---

### Задание 1.5
Создайте пустой класс без атрибутов. Используя `setattr` добавьте атрибут `version` с значением 100, после чего сделайте вывод на экран любым способом.

Далее реализуйте удаление атрибута через `delattr`, удалите его и сделайте вывод на экран.

##### Ваша реализация кода:
```python
class Test:
    pass
```

---

### Задание 1.6
Что выводит `__dict__` когда мы вызываем его обращаясь к объекту?

##### Варианты ответа:
0) Используемые функции
1) Словарь атрибутов объекта
2) Аргументы объекта
Ваш ответ: 1

---

### Задание 1.7
Разработчик создал экземпляр из класса, где использовался `__init__`. В дальнейшем он изменил значение уже в самом классе. Отразится ли это на данных всех созданных экземпляров?

##### Варианты ответа:
0) Нет, так как `__init__` и аргумент `self` создает объекты внутри своего пространства имен
1) Да, так как они будут ссылаться на одинаковую ячейку в памяти
Ваш ответ: 0

---

### Задание 1.8
Для чего нужен `self`?

##### Варианты ответа:
0) Для создания экземпляров класса
1) Чтобы привязать данные к конкретному экземпляру класса
2) Чтобы обращаться к глобальным атрибутам
Ваш ответ: 1

---

### Задание 1.9
Возможно ли использовать `getter` для записи данных?

##### Варианты ответа:
0) Да
1) Нет
Ваш ответ: 1

---

### Задание 2.0
Чем отличается `getter` и `setter`?

##### Варианты ответа:
0) Getter доступен только для чтения, а setter нужен для записи данных
1) Getter позволяет записывать данные, а setter используется для чтения и удаления данных
Ваш ответ: 0

---

### Задание 2.1
Зачем использовать Dunder методы `__get__` и `__set__`?

##### Варианты ответа:
0) Это позволяет реализовать свойства (property) более удобно
1) С помощью `__get__` и `__set__` можно обращаться к спискам используя индексы
2) Это необходимо для сериализации данных
Ваш ответ: 2
