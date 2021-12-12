# Motivational Poster Project

## Overview

Creating motivational posters is only a few clicks away. Making motivational posters with our website is quick and seamless-- just click the `Show Another Random Poster` button to make a new poster. Or, fuel your creative side and make your own poster by clicking `Make Your Own Poster`. Want to save your new creation to share with your friends? Just click `Save This Poster` and your new creations will be accessible via the `Show Saved Posters` button. It's that easy!

![alt text](https://ibb.co/tHbWXnh)

Alright, you're all set to create some amazing new posters. Time to get out there and create some motivation!


### Project Motivation

The Motivational Poster Project aims to teach new developers about the structure and function of the DOM and how JavaScript, CSS, and HTML work together to create functional and interactive web pages.


## Project Information
#### Code Style & Framework
* JavaScript
* HTML
* CSS
* Constructed and manipulated using ATOM text editor

#### Features
* Show Random Poster
* Create Your Own Poster
* Save and Delete Posters

#### Code Sample
The following is one example of code that played an integral role in our webpage:
```javascript
function showSaved() {
  savedPostersPage.classList.toggle("hidden");
  hideMain();
  savedPostersGrid.innerHTML = ``;
  for (var i = 0; i < savedPosters.length; i++) {
  savedPostersGrid.innerHTML += `
    <button id="delete-poster-button">
    <section class="mini-poster" id=${savedPosters[i].id}>
    <img src="${savedPosters[i].imageURL}">
    <h2>${savedPosters[i].title}</h2>
    <h4>${savedPosters[i].quote}</h4>
    </section>
    </button>
    `;
  }
}
```

### Installation

1. To edit this repo fork and clone to local
2. `cd` into repository
3. Open in text editor
4. To view webpage, run the command `open index.html` in your terminal

### Credits

For original repo [click here](https://github.com/turingschool-examples/hang-in-there-boilerplate)
