# fullstack-dev-exercises

## Exercises for lecture #1

- Виконайте інсталяцію Visual Code
- Виконайте інсталяцію git
- Виконайте початкове налаштування Git
- Зареєструйтесь на github
- Створіть новий репозиторій з ім’ям свого облікового запису.

- В корені проєкту виконайте команду:

git remote add origin https://github.com/<ім’я вашого облікового запису>/<ім’я вашого облікового запису>.github.io

### Виконайте наступні кроки
1. В корені проєкту:
	- створіть файл README.md 
	- створіть файл index.html

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>

</body>
</html>

```
На сайті https://favicon.io/ згенеруйте файл favicon.ico та розмістить його до кореня проєкту.
Відредагуйте файл index.html

```html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <!-- Додайте тут іконку для вашого сайту -->
	<link rel="shortcut icon" href="/favicon.ico" type="image/x-icon">
</head>
<body>

</body>
</html>

```

2. Створіть директорію exercises

	- В середині exercises створіть файл README.md
	- В середині exercises створіть піддиректорію lecture-01
	- В середині lecture-01 створіть файли index.html та README.md

**Результатом повинна стати така структура:**
```
├── exercises
│   ├── lecture-01
│   │   ├── index.html
│   │   └── README.md
│   └── README.md
├── index.html
├── LICENSE
└── README.md

```

3. Відредагуйте файл exercises/README.md

```
## Мої домашні вправи
```

4. Відредагуйте файл exercises/lecture-01/README.md

```
## Домашні вправи до лекції 1
```

5. Відкрийте термінал та перейдіть у корінь проєкту. Виконайте наступні команди з терміналу
	- git add .
	- git commit -m "added exercise 1"
	- git push origin main

6. В браузері викличте https://<ім’я вашого облікового запису>/<ім’я вашого облікового запису>.github.io 

