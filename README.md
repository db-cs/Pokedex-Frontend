# Pokedex-Frontend

For this project you will be using the [PokeAPI](https://pokeapi.co/) as a backend and building a frontend Pokedex to serve the data to users.

## Apply what you've learned

The goal here is not to reinvent the wheel. We will get into some more complex examples later, but for now I want you to use what you've learned from the Pinboard project to build out this app. Here are some key things I will look for:

- [ ] Code is well organized into atleast three separate files (index.html, style.css, and script.js).
- [ ] Data is fetched from the API in at least 3 different ways (3 different purposes).
- [ ] CSS is used to style the project.
- [ ] JavaScript is used to create elements, inject content, and render in the browswer.
- [ ] JavaScript and is used with a form to allow the user to interact by searching.

## Fetching Data

With most modern web browser ([https://caniuse.com/?search=fetch](https://caniuse.com/?search=fetch)) you can use the fetch method to get a resource accross the network. The full documentation can be found at [https://developer.mozilla.org/en-US/docs/Web/API/fetch](https://developer.mozilla.org/en-US/docs/Web/API/fetch). Here's a simple example of how you might use this with the PokeAPI:

```javascript
fetch("https://pokeapi.co/api/v2/pokemon/ditto")
  .then((response) => response.json())
  .then((data) => console.log(data))
  .catch((err) => console.log(err));
```
