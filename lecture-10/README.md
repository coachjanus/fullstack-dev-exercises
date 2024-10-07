# fullstack-dev-exercises

## Exercises for lecture #10 - Animations


1. В середині exercises створіть піддирексторію lecture-10. В середині lecture-10 створіть файли index.html та css/main.css. 

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en" >

<head>
  
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Transform explanation</title>

  <link rel="stylesheet" href="css/main.css">
  
</head>

<body>
  <div class="box">
        <div class="scale-element">
            Цей елемент має 20 пікселів у ширину та 20 пікселів у висоту, але, якщо для функції масштабування встановлено значення 10, він тепер має 100 пікселів у ширину та 400 пікселів у висоту. Ця властивість також впливає на текст, відступи та поля.
        </div>
    </div>

  <div class="box">
    <div class="skew-element">
    </div>
    <div class="skew-element">
    </div>
    <div class="skew-element">
    </div>
  </div>
  
  <div class="box">
    <div class="rotate-element">
    </div>
    <div class="rotate-element">
    </div>
    <div class="rotate-element">
    </div>
  </div>

  <div class="box">

    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusamus porro officia, quae, explicabo deleniti quasi molestias dolorum non ad pariatur. Illo, inventore at. Odio iure adipisci quisquam, molestias impedit quo.</p>

    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Doloribus unde, quis. Natus quasi, eveniet corporis facere laboriosam voluptatem ad blanditiis, temporibus, laborum voluptate possimus beatae illo. Illo molestiae, iure blanditiis.</p>

    <div class="square"></div>
    
    <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum sit aperiam odit libero soluta delectus voluptatibus saepe laboriosam maiores, quas, fuga vitae. Suscipit eum assumenda hic sunt, debitis voluptatum odit.</p>

  
  </div>
</body>

</html>

```

## файл css/main.css:

```css

* {
    margin: 0;
}

body, html {
  height: 100%;
}

.box {
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 2rem;
}

.scale-element {
  background-color: #0074d9;
  height: 20px;
  width: 20px;
  font-size: 1px;
  padding: 1px;
  color: white;
  line-height: 2px;
}

.skew-element {
  display: inline-block;
  background-color: #0074d9;
  height: 100px;
  width: 100px;
  font-size: 1px;
  padding: 1px;
  color: white;
  margin-right: 5px;
  margin-left: 5px;
  animation-direction: alternate;
  opacity: 0.7;
}



@keyframes skew {
  0% {

  }
  100% {

  }
}

.rotate-element {
  display: inline-block;
  background-color: #0074d9;
  height: 100px;
  width: 100px;
  font-size: 1px;
  padding: 1px;
  color: white;
  margin-right: 5px;
  margin-left: 5px;
  opacity: 0.7;
}

@keyframes roll {
  0% {
    
  }
  100% {
    
  }
}

.square {
  height: 100px;
  width: 100px;
  background-color: #3d9970;
  display: flex;
  text-align: center;
  justify-content: center;
  align-content: center;
  color: white;
  padding: 5px;

  animation-direction: alternate;
}


@keyframes shimmy {
  0% {

  }
  100% {

  }
}
```

  - збільшити масштаб селектора scale-element у 10 разів
  - встановити нахил елементу .skew-element у 20deg
  - створити keyframes з ім'ям skew. У фреймі 100% визначити нахил елементу ліворуч на 20deg. У фреймі 0% визначити нахил елементу праворуч на 20deg.
  - призначити елементу .skew-element властивісь animation, що иає назву skew, тримає 3 секунди та ніколи не спиняється

  - поверніть елемент .rotate-element на 30deg
  - створити keyframes з ім'ям roll. У фреймі 100% визначити поворот елементу на 360deg. У фреймі 0% визначити поворот елементу на 0deg.
  - призначити елементу .rotate-element властивісь animation, що має назву roll, тримає 3 секунди та ніколи не спиняється

  - створити keyframes з ім'ям shimmy. У фреймі 0% визначити переиіщення у точку (0, 0). У фреймі 100% визначити переиіщення у точку (20px, 50px).
  - призначити елементу .square властивісь animation, що має назву shimmy, тримає 3 секунди та ніколи не спиняється
