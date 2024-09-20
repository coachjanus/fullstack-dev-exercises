# fullstack-dev-exercises

## Exercises for lecture #3 Каскадні стилі сторінок (CSS)


1. В середині exercises створіть піддирексторію lecture-03. В середині lecture-03 створіть файли index.html та README.md

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lesson 3 challenges</title>

    <link rel="shortcut icon" href="./favicon.ico" type="image/x-icon">

</head>
<body>

</body>
</html>
```

2. Відредагуйте файл index.html
```html 

<!doctype html>
  <head>
	<!-- 
		Додайте тут елеиент style 
		В сепедині style визначте селектор p з властивістю color: red;
	-->
  </head>
  <body>
	<!-- 
		Додайте тут елеиент p з текстом This is my paragraph.
		визначте атрибут style для тега p зі значенням color: blue;
	-->

	<!-- 
		який колір буде мати текст This is my paragraph і чому.
	-->

  </body>
</html>
```

3. У наступному фпагменті випрвити помилки 
```html 
    <p>Звичайний, нудний абзац. Намагайтеся не заснути.</p>

    <p id="exciting">The most exciting paragraph on the page. One of a kind!</p>

    <div id="exciting">The most exciting paragraph on the page. One of a kind!</div>

	<style>
		#exciting {
			background: #f69d3c;
			border: 1px solid #696969;
			padding: 10px;
		}
	</style>
```


4. Чи буде змінна --bgColor видимою для елемента body. Яким буде фон елемента body і чому.

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lesson 3 challenges</title>
    <link rel="shortcut icon" href="./favicon.ico" type="image/x-icon">

    <!-- Додайте тут елеиент style: -->
    <style type="text/css">
    	
    	body {
			background: var(--bgColor);
		}

		div {
			--bgColor: limegreen;
		}

		/*
		 визначте для елементів p властивість фону таким чином:
			background: var(--bgColor);
		*/
    </style>

</head>
<body>

    <!-- ... -->

	<!-- Додайте тут 2 елеиенти div: -->
	<div>
		<h3>Div 1</h3>
	    <p>Paragraph 1</p>
	</div>

	<div>
		<h3>Div 2</h3>
	    <p>Paragraph 2</p>
	</div>

</body>
</html>
```

5. Створити файл css/main.css
	- Перейти до кореня персонального сайта
	- Створити файли css/main.css та css/base.css
	- Відредагувати файл index.html
		1. Підключити css/main.css за допомогою тега link
		2. Підключити css/base.css за допомогою правила @import


6. Виправити помилку у фпагменті
```css
	* {
		margin: 0;
		padding: 0;
	}

	/* more styles */
	@import url("my-imported-styles.css");

```


7. Відредагувати файл css/base.css
	- Визначити у глобальній області видимості змінну:
    	--accentColorMuted: hsl(300, 40%, 40%);
	- Встановити, за допомогою цієї змінної властивість color для елемента a


8. Відредагувати розділ footer
```html

<footer>
  <!-- створити тут секцію -->
  	<!-- створити тут div -->
      <h2>About</h2>
	  <!-- 
	  створити тут невпорядкований список з такмсм елементами 
	  	<a href="#">Services</a>
        <a href="#">Portfolio</a>
        <a href="#">Pricing</a>
        <a href="#">Customers</a>
        <a href="#">Careers</a>
	  -->
	
	<!-- створити тут div -->
      <h2>Resources</h2>
	  <!-- 
	  створити тут невпорядкований список з такмсм елементами 
	  	<a href="#">Docs</a>
        <a href="#">Blog</a>
        <a href="#">eBooks</a>
        <a href="#">Webinars</a>
	  -->

	<!-- створити тут div -->
      <h2>Contact</h2>
	  <!-- 
	  створити тут невпорядкований список з такмсм елементами 
	  	<a href="#">Help</a>
        <a href="#">Sales</a>
        <a href="#">Advertise</a>
	  -->

  
  <!-- Footer legal -->
  <!-- створити тут section -->
  <!-- 
	  створити тут невпорядкований список з такмсм елементами 
	  	<a href="#">Terms &amp; Conditions</a>
        <a href="#">Privacy Policy</a>
        &copy; 2024 Copyright Shopaholic Inc.
	  -->
</footer>
```