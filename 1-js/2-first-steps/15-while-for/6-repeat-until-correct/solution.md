

```js run demo
var num;

do {
  num = prompt("Введите число больше 100?", 0);
} while (num <= 100 && num != null);
```

Цикл `do..while` повторяется, пока верны две проверки:

1. Проверка `num <= 100` -- то есть, введённое число всё еще меньше `100`.
2. Проверка `num != null` -- значение `null` означает, что посетитель нажал "Отмена", в этом случае цикл тоже нужно прекратить.

Кстати, сравнение `num <= 100` при вводе `null` даст `true`, так что вторая проверка необходима.