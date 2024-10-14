# fullstack-dev-exercises

## Exercises for lecture #13 - DOM

1. В середині exercises створіть піддирексторію lecture-13. В середині lecture-13 створіть файли index.html та js/main.js. 

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>lecture №13 - об'єктна модель документа</title>
   <link rel="shortcut icon" href="/favicon.ico" type="image/x-icon">
   <link rel="stylesheet" href="css/main.css">
</head>
<body>

    <div class="container">
        <header>
            <h1 class='title' id='first-title'>First Title</h1>
        </header>
        
        <p id="p1">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Labore accusantium distinctio explicabo iure possimus natus obcaecati fugiat voluptas id, eveniet ab, voluptate repellat? Inventore voluptate perferendis sequi distinctio qui consectetur.
          <button>It's First Button</button>
        </p>
    </div>
    
    <div class="container">
        <header>
            <h1 class='title' id='second-title'>Second Title</h1>
        </header>
        
        <p id="p2">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Labore accusantium distinctio explicabo iure possimus natus obcaecati fugiat voluptas id, eveniet ab, voluptate repellat? Inventore voluptate perferendis sequi distinctio qui consectetur.
          <button>It's Second Button</button>
        </p>
    </div>
    
    <div class="container">
        <header>
            <h1 class='title' id='third-title'>Third Title</h1>
        </header>
        
        <p id="p3">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Labore accusantium distinctio explicabo iure possimus natus obcaecati fugiat voluptas id, eveniet ab, voluptate repellat? Inventore voluptate perferendis sequi distinctio qui consectetur.
        <button>It's Third Button</button>
      </p>
    </div>
    
    <div class="container">
        <header>
            <h1 class='title' id='fourth-title'>Fourth Title</h1>
        </header>
    
        <p id="p4">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Labore accusantium distinctio explicabo iure possimus natus obcaecati fugiat voluptas id, eveniet ab, voluptate repellat? Inventore voluptate perferendis sequi distinctio qui consectetur.
          <button>It's Fourth Button</button>
        </p>
    </div>

      <script type="module" src="js/main.js"></script>
</body>
</html>



```
## Вміст css/main.css:
```css
.first {
    color: red;
}
.second {
    color: blue;
}
.third {
    color: green;
    background-color: yellow;
}

.fourth {
    color: gray;
    
}
.border {
    border: solid red 1px;
}

.title {
    padding: 1rem 2rem;
    border: double 2px violet;
}
```

## файл js/main.js:

```js
'use strict';

const classes = ['first', 'second', 'third', 'fourth'];
```
1. Отримати перший абзац за допомогою **_document.querySelector('#id')_** за його ідентифікатором p1. Встановити для нього стиль background-color = "gold"
    

2. Отримати другий абзац за допомогою **_document.querySelector('#id')_** за його ідентифікатором p2. Встановити для нього стилі background-color:gold; color: blue; font-size: 2rem;

3. Отримати третій абзац за допомогою **_document.querySelector('#id')_** за його ідентифікатором p3. Призначити для нього клас third 

4. Отримати четвертий абзац за допомогою **_document.querySelector('#id')_** за його ідентифікатором p4. Призначити для нього класи fourth та border

5. Отримати першу кнопку за допомогою **_document.querySelector()_**. Призначити для неї стилі background-color:gold; color: blue;

6. Отримати другу кнопку за допомогою **_document.querySelector()_**. Виконати обробку події натискання на цю кнопку, що призводить до приховування параграфа p1.

7. Отримати третю кнопку за допомогою **_document.querySelector()_**. Виконати обробку події натискання на цю кнопку, що відображає прихований параграф p1.

8. Отримати четверту кнопку за допомогою **_document.querySelector()_**. Виконати обробку події натискання на цю кнопку, що переключає тему документа з світлої на темну і навпаки.
