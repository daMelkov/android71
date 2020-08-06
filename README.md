# Задача №1. Цепочка текста
## Задание:

ConstraintLayout предоставляет нам широкий набор инструментов графического оформления. Дополните свой калькулятор цепочкой текста с именем автора программы вокруг панели цифр.

## Выполнение

В созданном в предыдущих ДЗ калькуляторе нужно добавить фамилию автора.

Чтобы это сделать, нужно:
1. LinearLayout, который содержит панель кнопок, нужно обернуть в ещё один Layout.
2. В начале нового Layout вставить ConstraintLayout.
3. В ConstraintLayout вставить несколько TextView на каждую букву фамилии.
4. Созданные ConstraintLayout распределить по горизонтали равномерно.

> Цепочку текста организуйте с помощью Chain, рассмотренного в лекции и примера https://medium.com/@nomanr/constraintlayout-chains-4f3b58ea15bb

Чтобы распределить элементы равномерно, надо задать им chainStyle:

```app:layout_constraintHorizontal_chainStyle=”spread”
app:layout_constraintVertical_chainStyle=”spread”
```

![](screen.png)