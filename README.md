# Решение задач выложить на GitHub

## Задача 1
Реализовать счетчик на JavaScript, со следующим API:
- Начальное значение счетчика по умолчанию равно 1;
- Cчетчик должен обладать возможностью установить другое начальное значение;
- Cбросить значение в 1;
- Получить текущее значение счетчика.

Пример работы:

```js
function makeCounter() { /* ваш код */ }

var counter1 = makeCounter();

counter1();
console.log(counter1.get()); // 2
counter1.set(10);
counter1();
console.log(counter1.get()); // 11
console.log(counter1()); // 11
counter1.reset();
console.log(counter1.get()); // 1
```

## Задача 2
Реализовать строковый буфер на JavaScript, со следующим API:
- Создание объекта: ```var buffer = makeBuffer();```.
- Вызов ```makeBuffer``` должен возвращать такую функцию buffer, которая при вызове ```buffer(value)``` добавляет значение в некоторое внутреннее хранилище, а при вызове без аргументов ```buffer()``` – возвращает его.

Пример работы:
```js
function makeBuffer() { /* ваш код */ }

var buffer1 = makeBuffer();

// добавить строку
buffer1(' Hello');
buffer1(' World');
buffer1('!');
alert( buffer1() ); // Hello World!

// добавить число
var buffer2 = makeBuffer();
buffer2(0);
buffer2(1);
buffer2(0);
alert( buffer2() ); // '010'
```