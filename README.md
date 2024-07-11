# Cash Register 🚀

## Project Description 📝

> Pokemon Search App build in HTML, CSS and javaScript it can search for pokemons from their ID or name.project.

### HTML:
```html

  <form role="search" id="search-form">
    <label for="search-input">Search for Pokemon Name or ID:</label>
    <input type="text" name="pokemon" id="search-input" required />
    <button id="search-button">Search</button>
  </form>

```
### CSS:
```css

main {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

h1 {
  color: #f5f6f7;
  font-size: 16px;
  text-align: center;
}



```
### JS:
```javascript

const getPokemon = async () => {
  try {
    const pokemonNameOrId = searchInput.value.toLowerCase();
    const response = await fetch(
      `https://pokeapi-proxy.freecodecamp.rocks/api/pokemon/${pokemonNameOrId}`,
    );
    const data = await response.json();

    pokemonName.textContent = `${data.name.toUpperCase()}`;
    pokemonID.textContent = `#${data.id}`;
    weight.textContent = `Weight: ${data.weight}`;
    height.textContent = `Height: ${data.height}`;
    spriteContainer.innerHTML = `
    <img id="sprite" src="${data.sprites.front_default}" alt="${data.name} front default sprite">
  `;


```

## Demo 📸



## Technologies Used 🛠️

- HTML
- CSS
- JavaScript

## Features ⭐

- Building Pokemon-Search-App

## Author 👩‍💻


- LinkedIn: (linkedin.com/in/hasina-rahmani-4a21a9311)
- Email: (hasinarahmani548@gmail.com)
- GitHub:(https://github.com/Hasinarahman/Pokemon-Search-App)


