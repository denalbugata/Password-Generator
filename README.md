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

```javascript
// Define an array of characters to use for the password
const charSet = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()_+-=[]{}|;':\"<>,.?/~`";
```
<b>Step 2: Define a function to generate a random password.</b>

```javascript
// Create a function to generate a random password
function generatePassword(length) {
  let password = "";

  // Loop through the character set to create a password of the specified length
  for (let i = 0; i < length; i++) {
    password += charSet.charAt(Math.floor(Math.random() * charSet.length));
  }

  // Return the generated password
  return password;
}
```

<b>Step 3: Call the function to generate a random password with a specified length.</b>

```javascript
// Call the generatePassword function to get a random password
let password = generatePassword(12);

// Log the generated password to the console
console.log(password);
```

<b> The final result should look like this:</b>
```javascript
// Define an array of characters to use for the password
const charSet = "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789!@#$%^&*()_+-=[]{}|;':\"<>,.?/~`";

// Create a function to generate a random password
function generatePassword(length) {
  let password = "";

  // Loop through the character set to create a password of the specified length
  for (let i = 0; i < length; i++) {
    password += charSet.charAt(Math.floor(Math.random() * charSet.length));
  }

  // Return the generated password
  return password;
}

// Call the generatePassword function to get a random password
let password = generatePassword(12);

// Log the generated password to the console
console.log(password);
```
