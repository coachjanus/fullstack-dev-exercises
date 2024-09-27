# fullstack-dev-exercises

## Exercises for lecture #6 Box Model

1. В середині exercises створіть піддирексторію lecture-06. В середині lecture-06 створіть файли index.html та css/main.css. 

Є два бокси - box1 та box2

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exercises for lecture #6</title>
    <link rel="shortcut icon" href="/favicon.ico" type="image/x-icon">

    <link rel="stylesheet" type="text/css" href="css/main.css">

</head>

<body class="body">
    
    <div class="box box1">I use the standard box model.</div>
    <div class="box box2">I use the alternate box model.</div>
    
    <div class="box">
      <p>
        Veggies es bonus vobis,
        <span>proinde vos postulo</span>
        essum magis kohlrabi welsh onion daikon amaranth tatsoi tomatillo melon
        azuki bean garlic.
      </p>

      <p>
        Gumbo beet greens corn soko endive gumbo gourd. Parsley shallot
        courgette tatsoi pea sprouts fava bean collard greens dandelion okra
        wakame tomato. Dandelion cucumber earthnut pea peanut soko zucchini.
      </p>
    </div>
</body>
</html>
```

Відредагуйте файл css/main.css:

```css
.box {
  border: 5px solid rebeccapurple;
  background-color: lightgray;
  padding: 40px;
  margin: 40px;
  width: 300px;
  height: 150px;
}

.box span {
    background-color: pink;
    border: 5px solid black;
    padding: 1em;
}

```

    - Перший бокс box1 повмнен використовувати стандартну боксову модель, другий box2 – альтернативну боксову модель. 


    - Додайте до box2 нвступні властивості:
        - Чорну пунктирну рамку розміром 5 пікселів.
        - Верхнє поле 20 пікселів.
        - Праве поле 1em.
        - Нижнє поле 40 пікселів.
        - Ліве поле 2 em.
        - Підкладку з усіх боків 1ем.


    - Вбудований елемент span має поле, відступ і рамку. Однак лінії вгорі та внизу перекривають його. Золбіть так, щоб інші рядки дотримувалися розміру полів, відступів і рамок, зберігаючи при цьому вбудований елемент span.

    - Створіть div для всього вмісту сторінки та відцентруйте його посередині сторінки. Додайте рамку та відступ до цього div.
