<h1>Random Password Generator</h1>

<h2>Description</h2>
This code generates a random password in JavaScript. A string of characters is defined that will be used to generate the password. A function called generatePassword is then defined which takes in a length argument. Within the function, an empty string called password is defined, and a for loop is used to iterate the specified length of times. Within the loop, a random index is selected from the characters string, and the corresponding character is added to the password string. The function returns the password string. Finally, the function is called with a length of 16, and the generated password is logged to the console.
<br />


<h2>Languages and Utilities Used</h2>

- <b>JavaScript</b> 

<h2>Environments Used </h2>

- <b>Windows 11</b>

<h2>Program Walkthrough:</h2>

<b>Step 1: Create an array of characters to choose from.</b>

```python
var characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()_+-=";
```
<b>Step 2: Define a function to generate a random password.</b>

```python
function generatePassword(length) {
    var password = "";
    for (var i = 0; i < length; i++) {
        var randomIndex = Math.floor(Math.random() * characters.length);
        password += characters[randomIndex];
    }
    return password;
}
```

<b>Step 3: Call the function to generate a random password with a specified length.</b>

```python
var password = generatePassword(16);
console.log(password);
```

<b> The final result should look like this:</b>
```python
var characters = "abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789!@#$%^&*()_+-=";

function generatePassword(length) {
    var password = "";
    for (var i = 0; i < length; i++) {
        var randomIndex = Math.floor(Math.random() * characters.length);
        password += characters[randomIndex];
    }
    return password;
}

var password = generatePassword(16);
console.log(password);
```
