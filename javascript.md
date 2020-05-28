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
