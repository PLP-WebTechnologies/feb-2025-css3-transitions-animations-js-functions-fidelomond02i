# CSS3 Transitions, Animations, and Advanced JavaScript Functions

## Objectives

Create smooth CSS transitions and animations.
Use JavaScript functions for dynamic behavior.
Implement local storage for data persistence.

## Instructions
Add CSS animations to elements like buttons or images.

>[!NOTE]
> - Write a JavaScript function that:
> - Stores and retrieves user preferences using localStorage.
> - Implements an animation triggered by user actions.

## Tasks

Create a CSS animation.
Store data in localStorage.
Apply JavaScript to trigger animations.


.button {
  background-color: #4CAF50;
  color: white;
  padding: 15px 32px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin: 4px 2px;
  cursor: pointer;
  border: none;
  border-radius: 12px;
  transition: background-color 0.3s, color 0.3s;
}

.button:hover {
  background-color: #45a049;
  color: white;
}
To store data in localStorage using JavaScript, you can use the localStorage object. For example, you can store a user’s preferences like this:
function storeUserPreferences(preferences) {
  localStorage.setItem("userPreferences", JSON.stringify(preferences));
}

function getUserPreferences() {
  return JSON.parse(localStorage.getItem("userPreferences"));
}
To apply JavaScript to trigger animations, you can use event listeners. For example, you can add the following code to your JavaScript file to trigger an animation when a button is clicked:
const button = document.querySelector(".button");

button.addEventListener("click", function() {
  const preferences = getUserPreferences();
  // Do something with the user's preferences
  // For example, change the button's color
  button.style.backgroundColor = preferences.color;
});
Happy Coding! 💻✨
