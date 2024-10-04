# fullstack-dev-exercises

## Exercises for lecture #9 Чуйний дизайн

1. В середині exercises створіть піддирексторію lecture-09. В середині lecture-09 створіть файли index.html та css/main.css. 

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="css/main.css">
  <title>Exercises for lecture #9</title>
</head>
<body>
  
 <div class="container">
   <div class="grid-container">
     <div class="header grid-item red">
       <h1>Чуйний дизайн</h1>
       <p>Lorem ipsum dolor sit amet.</p>
     </div>
     <div class="sidebar grid-item blue">
       <h2>Sidebar</h2>
       <ul>
        <li>List Item 1</li>
        <li>List Item 2</li>
        <li>List Item 3</li>
        <li>List Item 4</li>
        <li>List Item 5</li>
        <li>List Item 6</li>
       </ul>
     </div>
     <div class="main grid-item green">
       <h2>Main Content</h2>
       <p>This text has a font size of 20px at viewport width of 768px and font size of 36px when viewport width is 1920px. But if the viewport width is less than 768px, the font-size won't get lower than 16px and if the viewport width is more than 1920px font size will stop scaling at 48px. </p>

       <p>This text has a font size of 20px at viewport width of 768px and font size of 36px when viewport width is 1920px. But if the viewport width is less than 768px, the font-size won't get lower than 16px and if the viewport width is more than 1920px font size will stop scaling at 48px. </p>
      </div>
      <div class="footer grid-item orange">
        <h3>Footer</h3>
          <p>This text has a font size of 20px at viewport width of 768px and font size of 36px when viewport width is 1920px. But if the viewport width is less than 768px, the font-size won't get lower than 16px and if the viewport width is more than 1920px font size will stop scaling at 48px. </p>
      </div>
    </div>
  </div>

</body>
</html>

```

## файл css/main.css:

```css

  * {
    margin: 0;
  }

  body {
    color: #000;
    background: #fff;
    font-family: Arial, sans-serif;
    padding: 1em;
  }

  .grid-container {
    display: grid;
    grid-gap: 20px;
    grid-template-areas:
        'header header header'
        'sidebar main main'
        'footer footer footer';
}

.header {
    grid-area: header;
}

.main {
    grid-area: main;
}

.sidebar {
    grid-area: sidebar;
}

.footer {
    grid-area: footer;
}

```

  - Використовуючи функції clamp() та calc(), розрахуйте font-size, дотримуючись таких вимог:
  - Якщо ширина вікна перегляду становить 768 пікселів, розмір шрифту має дорівнювати 20 пікселям
  - Якщо ширина вікна перегляду перевищує 768 пікселів, розмір шрифту масштабується пропорційно
  - При 1920 пікселях розмір шрифту має дорівнювати 36 пікселями
  - Для екранів, менших за 768 пікселів, розмір шрифту не має бути меншим за 16 пікселів
  - Для екранів, розмір яких перевищує 1920 пікселів, розмір шрифту не має перевищувати 48 пікселів
  - Створіть "Mobile First" media-запит, що перетворює макет іменованих областей з 2-х колонок на 1 колонку, при переході через контрольну точку 786px
