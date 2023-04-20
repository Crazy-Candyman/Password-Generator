# Random Password Generator

## About the Project

This is a web app that generates random passwords. The web app generates two strings of passwords. Each string is 15 characters long, are case-sensitive, and consists of symbols, numbers, and letters.

## Desktop / Mobile Screenshots

![](/screenshots/password_gen_desktop.png)
![](/screenshots/password_gen_mobile.png)

## Links

Live URL: [Preview Site](https://crazy-candyman.github.io/Password-Generator/)

## Built With

    - HTML
    - CSS
    - JavaScript

**JavaScript code from the solution**

```javascript
let btn = document.getElementById("btn");
let boxOne = document.getElementById("box-one");
let boxTwo = document.getElementById("box-two");

btn.addEventListener("click", function generator() {
  let generatorOne = "";
  let generatorTwo = "";
  for (let i = 0; i < 15; i++) {
    generatorOne += characters[Math.floor(Math.random() * characters.length)];
    generatorTwo += characters[Math.floor(Math.random() * characters.length)];
  }

  boxOne.textContent = generatorOne;
  boxTwo.textContent = generatorTwo;
});
```

## Atrribution

This is a solo project by Scrimba that challenges a students skills upon completing the Learn JavaScript Course.

Challenged by Scrimba <br/>
Created by [@Crazy-Candyman](https://github.com/Crazy-Candyman)
