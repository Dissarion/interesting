# Вопросы с собеседований 

### Что выведет следующий код: 

```javascript
for (var i = 0; i < 3; i++) { 
  setTimeout(function() { 
    consolelog(i); 
  }, 1000); 
} 
```
 
> Как сделать так, чтобы выводило 1,2,3. Есть два способа: через IIFE и через let. 

### Написать реализацию функции lodash/debounce. 

### Алгоритм поиска
Есть поисковый инпут. Надо реализовать поиск по нескольким вхождениям. Вхождения разделяются пробелом. Подсказки выдаются по всем вхождениям сразу. Подсказки не могут повторяться. 

### Что выведется в консоль? 

```javascript
function Person(name) {
  this.name = name;
}

const john = new Person('john');

Person.prototype = {
  getName: function () {
    return this.name;
  }
};

const susan = new Person('susan');

console.log(john.getName());
console.log(susan.getName());
```

## А так?
```javascript
function Person(name) {
  this.name = name;
}

const john = new Person('john');

Person.prototype.getName = function () {
    return this.name;
  }

const susan = new Person('susan');

console.log(john.getName());
console.log(susan.getName());
```
### Что выведет в консоль?
```javascript
const user = { name: 'John' };
const position = { title: 'Frontend' };

user.position = position;
user.position.salary = 10000;

position.title = 'Backend';

console.log(user);
console.log(user.position);
console.log(position);
```

### Чем отличаются примитивы от объектов?
### Что выведет typeof на каждом типе?
### Как работает асинхронность?
### Сколько состояний у промиса?
### Как работает async/await?
### Зачем нужна вся эта асинхронщина? Почему не можем просто спросить данные и нарисовать синхронно?
### Как работает Event Loop?
### Как работают таски и микротаски?
### Как работает наследование в JavaScript?




### Написать функцию сравнения
```javascript
function whatIs(arg) {
    const isNull = // ?
    const isObject = // ?
    const isArray = // ?
    const isNaN = // ?
    

    if (isObject) return 'object';
    if (isArray) return 'array';
    if (isNull) return 'null';
    if (isNaN) return 'nan';
}
```

### Что выведут элементы
```javascript
var f = [];

f[100] = 100;
console.log(f.lenght) // ?

const arr = new Array(500);

arr.map(console.log) // ?

for (let i = 0; i < arr.length; i++) console.log(arr[i]); // ?
```


### В каком порядке выведутся логи
```javascript
let loading = true;

setTimeout(() => {
    loading = false;
    console.log('1', loading); // ?
}, 0);

Promise.resolve(() => {
    setTimeout(() => {
        loading = false;
        console.log('2', loading); // ?
    }, 0);
})

// Promise.resolve(loading = false);

while(loading) {
    console.log('loading ...'); // ?
}

setTimeout(() => {
    loading = false;
    console.log('3', loading); // ?
}, 0);
```
 
### Напиши функцию проверки строки на палиндром «А муза рада музе без ума да разума» за один цикл, игнорируя пробелы и регистр

```javascript
function palindrome(str) {}
```

### Написать функцию counter() каждый вызов которой увеличивает счётчик и возвращает результат

```javascript
function counter() {}

const c = counter();

c() // 1
c() // 2
c() // 3

c.reset() // и добавить возможность сбросить счетчик

c() // 1
```
    
    
