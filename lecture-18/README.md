# fullstack-dev-exercises

## Exercises for lecture #18 - Template

1. В середині exercises створіть піддирексторію lecture-18. В середині lecture-18 створіть файли index.html, css/main.css та js/main.js. 

## файл index.html:

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Profile Card</title>  
    <link rel="stylesheet" href="css/main.css">
    
  </head>
  <body>
    <div id="profile-cards-container" class="profile-cards-container">
      <!-- Profile cards will be appended here -->
    </div>
    <template id="profile-card-template">
      <div class="profile-card">
        <img src="" alt="Profile Picture" class="profile-picture" />
        <div class="profile-title"></div>
        <div class="profile-job-title"></div>
        <div class="profile-description"></div>
      </div>
    </template>
    <script type="module" src="js/main.js"></script>
  </body>
</html>

```
## Вміст css/main.css:
```css

  .profile-cards-container {
        display: flex;
        flex-wrap: wrap;
        gap: 16px;
        justify-content: center;
  }
  .profile-card {
        border: 1px solid #ccc;
        border-radius: 8px;
        padding: 16px;
        margin: 16px;
        margin-top: 80px;
        box-shadow: 2px 2px 12px rgba(0, 0, 0, 0.1);
        max-width: 300px;
        text-align: center;
        font-family: Arial, sans-serif;
  }
  .profile-card img {
        border-radius: 50%;
        width: 100px;
        height: 100px;
        object-fit: cover;
        margin-bottom: 16px;
  }
  .profile-card .profile-title {
        font-size: 1.2em;
        font-weight: bold;
        margin-bottom: 8px;
  }
  .profile-card .profile-job-title {
        font-size: 1em;
        color: #777;
        margin-bottom: 16px;
  }
  .profile-card .profile-description {
        font-size: 0.9em;
        color: #555;
  }
```

## файл js/main.js:

```js
'use strict';

// Example profile data
const profiles = [
  {
    pictureUrl: "img/adna_mask.jpg",
    name: "Edna Mask",
    jobTitle: "Software Engineer",
    description: "Experienced in developing scalable web applications.",
  },
  {
    pictureUrl: "img/peter_cat.jpg",
    name: "Peter Cat",
    jobTitle: "Product Manager",
    description: "Guides product vision, strategy, and success.",
  },
  {
    pictureUrl: "img/grace_picasso.jpg",
    name: "Grace Picasso",
    jobTitle: "UX Designer",
    description: "Passionate about creating user-friendly designs.",
  },
];


```
- створити багаторазовий компонент картки профілю за допомогою шаблонів HTML і JavaScript.

