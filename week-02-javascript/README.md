# Week 2: JavaScript

## JavaScript in the browser

JavaScript adds behaviour to web pages. Place code inside `<script>` tags, commonly near the end of the HTML body. The browser developer console helps inspect output and errors.

```html
<script>
  console.log("Hello, SheCodes!");
</script>
```

## Variables and strings

`let` declares a variable. Strings use quotation marks; numbers can be written without quotation marks. Assigning a new value to an existing `let` variable does not require repeating `let`.

```js
let city = "Kempton Park";
let country = "South Africa";
let sentence = "I am from " + city + " in " + country;
console.log(sentence);
```

String concatenation joins values using `+`.

## Alerts and prompts

`alert()` displays a message; `prompt()` asks the user for input and returns the entered text or `null` if cancelled.

```js
let firstName = prompt("What is your first name?");
alert("Hello " + firstName);
```

## Conditional statements

Use `if`, `else if`, and `else` to run code based on conditions. `===` compares equality without type conversion, `!==` compares inequality, `&&` means AND, and `||` means OR.

```js
let age = 18;
if (age >= 18) {
  alert("You can apply");
} else {
  alert("Sorry, you cannot apply yet");
}
```

Conditions can also be nested when needed. Code comments use `//` or `/* ... */`.

## Functions

Functions group reusable instructions and run when called.

```js
function greetUser() {
  alert("Hello!");
}
greetUser();
```

## DOM selectors and events

`document.querySelector()` selects the first matching element, while `document.querySelectorAll()` selects all matches. An event listener can run a function when a button is clicked. `innerHTML` can update the selected element's content.

```js
function updateHeading() {
  document.querySelector("h1").innerHTML = "Welcome!";
}
let button = document.querySelector("button");
button.addEventListener("click", updateHeading);
```

## Related projects

- [Weather app](../projects/weather-app/)
- [Application page](../projects/application-page/)
