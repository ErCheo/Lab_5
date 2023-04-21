<h1 style="text-align: center;">МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ РОССИЙСКОЙ ФЕДЕРАЦИИ ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ «САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</h1>
<p style="text-align: center;">Лабораторная работа №5</p>
<p style="text-align: center;">"JS"</p>
<br>
<p style="text-align: right;">Работу выполнила Чёо Эрика Ильинична</p>
<p style="text-align: right;">Работу проверил Соболев Евгений Игоревич</p>

___

### **Цели и задачи**:
1. Создайте переменную str и присвойте ей значение 'hdfgv'. Обращаясь к отдельным символам этой строки выведите на экран символ 'h', символ 'd', символ 'v'.
2. Напишите скрипт, который считает количество секунд в часе.
3. Переделайте приведенный код так, чтобы в нем использовались операции +=, -=, *=, /=, ++, --. Количество строк кода при этом не должно измениться. Код для переделки:
```javascript
var num = 1;
num = num + 12;
num = num - 14;
num = num * 5;
num = num / 7;
num = num + 1;
num = num - 1;
alert(num);
```
4. Создайте переменную num и присвойте ей значение 3. Выведите значение этой переменной на экран с помощью метода alert.
5. Создайте переменные a=10 и b=2. Выведите на экран их сумму, разность, произведение и частное (результат деления).
6. Создайте переменные c=15 и d=2. Просуммируйте их, а результат присвойте переменной result. Выведите на экран значение переменной result.
7. Создайте переменные a=10, b=2 и c=5. Выведите на экран их сумму.
8. Создайте переменные a=17 и b=10. Отнимите от a переменную b и результат присвойте переменной c. Затем создайте переменную d, присвойте ей значение 7. Сложите переменные c и d, а результат запишите в переменную result. Выведите на экран значение переменной result.
9. Напишите скрипт, который считает количество секунд в часе, в сутках, в месяце.
10.	Создайте три переменные - час, минута, секунда. С их помощью выведите текущее время в формате 'час:минута:секунда'.
11.	Создайте переменную, присвойте ей число. Возведите это число в квадрат. Выведите его на экран.
12.	Напишите однострочное решение, которое вычисляет сумму квадратных корней для всех чётных чисел целочисленного массива.
13.	Яблоко стоит 1.15, апельсин стоит 2.30. Сколько они стоят вместе – чему равна сумма 1.15 + 2.30 с точки зрения JavaScript?
14.	Какое будет выведено значение: let x = 5; alert(x++); ?
15.	Чему равно такое выражение: `[ ] + false - null + true` ?
16.	Что выведет этот код: 
```javascript
let y = 1; 
let x = y = 2; 
console.log(x); 
```
17.	Чему равна сумма `[ ] + 1 + 2`?
18.	Создайте переменные a6, a7, a8, a9, a10. Поместите в них результат выражений: 5 % 3, 3 % 5, 5 + '3', '5' - 3, 75 + 'кг'
19.	Напишите скрипт, который находит площадь прямоугольника высота 23см. (в числовую переменную height), шириной 10см (в числовую переменную width), значение площади должно хранится в числовой переменной s.
20.	Напиши скрипт, который находит объем цилиндра высотой 10м (переменная heightC) и диаметром основания 4м (dC), результат поместите в переменную v.
21.	Даны размер ипотечного кредита (S — 2 млн.руб), процентная ставка (p  — 10%), кол-во лет (years — 5). Найти переплату по кредиту, значение переплаты должно содержаться в переменной perepl.
22.	Определите переменные str, num, flag и txt со значениями «Привет», 123, true, «true». При помощи оператора определения типа убедитесь, что переменных принадлежат типам: string, number, boolean.
23.	Дано число, необходимо вернуть противоположное число.

**Задачи на Codewars:**

1. https://www.codewars.com/kata/56530b444e831334c0000020
2. https://www.codewars.com/kata/583710ccaa6717322c000105
3. https://www.codewars.com/kata/5a805d8cafa10f8b930005ba
4. https://www.codewars.com/kata/5763bb0af716cad8fb000580
5. https://www.codewars.com/kata/578a8a01e9fd1549e50001f1
6. https://www.codewars.com/kata/57eae20f5500ad98e50002c5

___

**Задание 1**
```javascript
var str = "hdfgv"
document.getElementById("z1").innerHTML = str[0] + " " + str[1] + " " + str[4];
```
**Задание 2**
```javascript
document.getElementById("z2").innerHTML = 60*60 + " секунд в часе";
```
**Задание 3**
```javascript
var num = 1;
num += 12;
num -= 14;
num *= 5;
num /= 7;
num ++;
num --;
function myFunction_1 () {
    alert(num);
}
```
**Задание 4**
```javascript
function myFunction_2 () {
    var num = 3;
    alert(num);
}
```
**Задание 5**
```javascript
var a = 10, b = 2;
const mas_1 = [a + b, a - b, a * b, a / b];
const mas_2 = ["Сумма: ", "Разность: ", "Произведение: ", "Частное: "];
let text = "<ul>";
for (let i = 0; i < mas_1.length; i++) {
  text += "<li>" + mas_2[i] + mas_1[i] + "</li>";
}
text += "</ul>";
document.getElementById("z5").innerHTML = text;
```
**Задание 6**
```javascript
var c = 15, d = 2, result = c + d;
document.getElementById("z6").innerHTML = "Сумма c и d: " + result;
```
**Задание 7**
```javascript
var a = 10, b = 2, c = 5;
document.getElementById("z7").innerHTML = "Сумма a, b и c: " + (a + b + c);
```
**Задание 8**
```javascript
var a = 17, b = 10, c = a - b,
    d = 7, result = c + d;
document.getElementById("z8").innerHTML = "result = " + result;
```
**Задание 9**
```javascript
const HaD = {hour: 60*60, day: 60*60*24};
const temp = [" (с) в часе, ", " (с) в сутках, ", ", (с) в месяце"];
const M = [60*60*24*28, 60*60*24*29, 60*60*24*30, 60*60*24*31];
let list = "<ul>";
for (let i = 0; i < M.length; i++) {
    list += "<li>" + "Если количество дней в месяце" + (28 + i) + ": " + HaD.hour + temp[0] + 
    HaD.day + temp[1] + M[i] + temp[2] + "</li>";
}
list += "</ul>";
document.getElementById("z9").innerHTML = list;
```
**Задание 10**
```javascript
const date = new Date();
hour = date.getHours();
minute = date.getMinutes();
second = date.getSeconds();
document.getElementById("z10").innerHTML = "Текущее время: " + hour + ":" + minute + ":" + second;
```
**Задание 11**
```javascript
let count = 5;
document.getElementById("z11").innerHTML = "5^2 = " + Math.pow(count, 2);
```
**Задание 12**
```javascript
document.getElementById("z12").innerHTML = [1,2,3,4,5,6,7,8,9].reduce( (sum, n) => sum + (n % 2? 0 : n)**0.5, 0 );
```
**Задание 13**
```javascript
let apple = 1.15, orange = 22.30;
document.getElementById("z13").innerHTML = "apple + orange = " + (apple + orange);
```
**Задание 14**
```javascript
let x = 5;
alert(x++);
```
**Задание 15**
```javascript
document.getElementById("z15").innerHTML = "[] + false - null + true = " + ([] + false - null + true);
```
**Задание 16**
```javascript
let y = 1, x = y - 2;
console.log(x);
```
**Задание 17**
```javascript
document.getElementById("z17").innerHTML = "[] + 1 + 2 = " + ([] + 1 + 2);
```
**Задание 18**
```javascript
let a6 = 5 % 3, a7 = 3 % 5, a8 = 5 + '3', a9 = '5' + 3, a10 = 75 + 'кг';
const mass = [a6, a7, a8, a9, a10];
let ul = "<ul>";
for (let i = 0; i < mass.length; i++) {
    ul += "<li>" + "a" + (6 + i) + " = " + mass[i] + "</li>";
  }
ul += "</ul>";
document.getElementById("z18").innerHTML = ul;
```
**Задание 19**
```javascript
class pr {
    constructor(height, width) {
        this.height = height;
        this.width = width;
    }

    S(height, width) {
        let s = this.height * this.width;
        return s;
    }
}
let rec = new pr(23, 10);
document.getElementById("z19").innerHTML = "Площадь прямоугольника = " + rec.S() + " см";
```
**Задание 20**
```javascript
class C {
    constructor(heightC, dC) {
        this.heightC = heightC;
        this.dC = dC;
    }

    V(heightC, dC) {
        let pi = 3.14, r = this.dC / 2, 
            v = pi * this.heightC * Math.pow(r, 2);
        return v;
    }
}
let ci = new C(10, 4);
document.getElementById("z20").innerHTML = "Объём цилиндра = " + ci.V() + " м";
```
**Задание 21**
```javascript
let S = 2000000, p = 10, years = 5;
perepl = S * ((years + 1) / 20) * (p / 100);
document.getElementById("z21").innerHTML = perepl;
```
**Задание 22**
```javascript
function Func() {
    let str = "Привет", num = 123, flag = true, txt = "true";
    const mas = [str, num, flag, txt];
    let text1 = "<ul>";
    for (let i = 0; i < mas.length; i++) {
        text1 += "<li>" + mas[i] + " is " + typeof mas[i] + "</li>";
    }
    text1 += "</ul>";
    return text1;
}
document.getElementById("z22").innerHTML = Func();
```
**Задание 23**
```javascript
function reverse(count) {
    return count * (-1);
}
document.getElementById("z23").innerHTML = reverse(10);
```

___

**<h3 style="text-align: center;">Вывод:</h3>**
После выполнения данной лабораторной работы я научилась пользоваться перменными и проводить операции над ними.
