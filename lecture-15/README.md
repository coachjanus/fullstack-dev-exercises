# fullstack-dev-exercises

## Exercises for lecture #15 - Storages

1. В середині exercises створіть піддирексторію lecture-15. В середині lecture-15 створіть файли index.html, css/main.css та js/main.js. 

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="shortcut icon" href="/favicon.ico" type="image/x-icon">
    <title>Todo app</title>
    <link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css'>
    <link rel="stylesheet" href="css/main.css">
</head>
<body>

    <div class="container">
        <div class="to-do-app">
          <h2>To-do App</h2>
          <br>
          <input type="text" id="item" placeholder="Enter to do item...">
          <br>
          <br>
          <button onclick="add()">Add Item <i class="fa-solid fa-plus"></i></button>
          <button onclick="del()">Clear all <i class="fa-solid fa-ban"></i></button>
        </div>
        <ul class="to-do-list"></ul>
    </div>

    <script type="module" src="js/main.js"></script>
</body>
</html>



```
## Вміст css/main.css:
```css
@import url("https://fonts.googleapis.com/css2?family=Asap&display=swap");
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
body {
  width: 100%;
  height: 100vh;
  background-color: #e0d6e9;
  font-family: "Asap", sans-serif;
}
.container {
  max-width: 405px;
  margin: 137px auto;
  padding: 20px;
  display: flex;
  flex-direction: column;
}
.to-do-app {
  width: 100%;
  padding: 20px;
  border-radius: 5px;
  background-color: whitesmoke;
  border: 1px solid #d3d3d3;
}
.to-do-app h2 {
  padding: 10px;
}
.to-do-app input {
  width: 250px;
  padding: 5px;
  border-radius: 5px;
  border: 1px solid #d3d3d3;
}
.to-do-app button {
  width: fit-content;
  padding: 5px;
  cursor: pointer;
  border: 1px solid #d3d3d3;
  border-radius: 5px;
  background-color: whitesmoke;
}
.to-do-app button:hover {
  background-color: rgba(0, 0, 0, 0.1);
}
li {
  font-size: 1.5rem;
}
.to-do-list {
  margin-top: 20px;
  margin-right: 5px;
  padding: 0 20px 10px 25px;
  display: flex;
  flex-direction: column;
  gap: 15px;
  list-style: none;
}
.to-do-list li{
  font-size: small;
  background-color: whitesmoke;
  padding: 20px;
}
```

## файл js/main.js:

```js
'use strict';


```
- Знайти елемент ul у длкументі та запам'ятати його у змінній ul.

- За допомогою JSON.parse прочитати елемент localStorage з ключем items та зберегти його в масиві itemsArray. Якщо елемент відсутній, створити його зі значенням [].

- Написати функцію addTask(text), що створює елемент li з властивістю textContent, яка дорівнює значенню, що передається за допомогою аргументу функції text. Кожний створений елемент li функція повинна додавати до елемента ul.

- Використовуючи метод forEach та функцію addTask, згенерувати вміст елемента ul, відображаючи його на сторінці.

- Знайти елемент input у документі та запам'ятати його у змінній input.

- Написати функцію add(), що додає до масиву itemsArray значення, введене користувачем в полі input, та зберігає цей масив у localStorage з ключем items, використовуючи метод JSON.stringify. Одночасно візуалізувати доданий елемент на сторінці, використовуючи функцію addTask. 

- Написати функцію del(), що чистить localStorage, масив itemsArray та значення властивості ul.innerHTML. 
