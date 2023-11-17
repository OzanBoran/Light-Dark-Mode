# Dark-Light Mode Toggle - JavaScript

This JavaScript file is responsible for handling the dark-light mode toggle functionality on the web page. It interacts with HTML elements, such as the toggle switch, navigation bar, images, and text box, to dynamically update styles based on the selected theme.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [JavaScript Methods](#javascript-methods)
- [Deployment](#deployment)

## Features

- Dark and light mode toggle functionality.
- Dynamically updates styles based on the selected theme.
- Uses local storage to remember the user's theme preference.

## Installation

Clone the repository to your local machine using Git:

```bash
git clone https://github.com/OzanBoran/Light-Dark-Mode
```

## Usage

The dark-light mode toggle script provides a seamless way to enhance user experience by allowing them to switch between dark and light themes. It's suitable for a wide range of web applications and websites.

## JavaScript Methods

### `imgMode(color)`

This function takes a `color` parameter and updates the source of three images accordingly. It is used to set the images for both dark and light modes.

### `darkMode()`

This function applies styles for the dark mode. It updates the background color of the navigation bar and text box, changes the toggle icon, and calls `imgMode` with the 'dark' parameter.

### `lightMode()`

This function applies styles for the light mode. It updates the background color of the navigation bar and text box, changes the toggle icon, and calls `imgMode` with the 'light' parameter.

### `switchTheme(event)`

This function is the main driver for toggling between dark and light modes. It checks the state of the toggle switch and dynamically updates the theme, saving the preference in the local storage. It then calls either `darkMode` or `lightMode` based on the selected theme.

## Event Listener

The `toggleSwitch` element has an event listener attached to it. When the switch changes state, the `switchTheme` function is called to handle the theme switch dynamically.

```javascript
// Event Listener
toggleSwitch.addEventListener('change', switchTheme);
```
This event listener ensures that the switchTheme function is invoked whenever the user interacts with the dark-light mode toggle switch. The function evaluates the state of the switch and adjusts the theme accordingly.

## Local Storage
The script includes a section that checks the local storage for the user's preferred theme. This is done to provide a consistent theme experience for users across different visits to the website.

This method ensures that when a user revisits the website, their previous theme preference is applied automatically. If a theme is found in the local storage, it sets the HTML attribute accordingly, updates the toggle switch state, and invokes the appropriate mode function (darkMode or lightMode). This way, the website maintains a consistent appearance based on the user's preferences.

## Deployment

The project is deployed and can be accessed online at: https://ozanboran.github.io/Light-Dark-Mode/

## Credits
- **Developer:** Ozan Boran
