# React Pokédex

A modern, responsive Pokédex application built with React that allows users to browse, search, and view detailed information about Pokémon using the [PokéAPI](https://pokeapi.co/).

![Pokédex App Screenshot]([https://raw.githubusercontent.com/username/react-pokedex/main/screenshot.png](https://raw.githubusercontent.com/benrigaud/react-pokedex/refs/heads/main/screenshot.png))

## 🚀 Features

- **Browse Pokémon**: Navigate through the complete list of Pokémon with pagination
- **Search Functionality**: Find Pokémon by name using the search bar
- **Detailed View**: View comprehensive information about each Pokémon including:
  - Base statistics
  - Type information (with color coding)
  - Physical characteristics
  - Abilities
- **Responsive Design**: Works on both desktop and mobile devices
- **Type-Based Styling**: Each Pokémon type has its own distinct color scheme

## 🛠️ Technologies

- [React](https://reactjs.org/) - UI library
- [React Router](https://reactrouter.com/) - For navigation
- [Vite](https://vitejs.dev/) - Build tool
- [Zustand](https://github.com/pmndrs/zustand) - State management
- [FontAwesome](https://fontawesome.com/) - Icons
- [CSS Modules](https://github.com/css-modules/css-modules) - For component-scoped styling
- [PokéAPI](https://pokeapi.co/) - Pokémon data source

## 📋 Prerequisites

- Node.js (v14.0.0 or higher)
- npm (v6.0.0 or higher) or yarn

## 🔧 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/username/react-pokedex.git
   cd react-pokedex
   ```

2. Install dependencies:
   ```bash
   npm install
   # or
   yarn
   ```

3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

4. Open your browser and visit:
   ```
   http://localhost:5173
   ```

## 🏗️ Project Structure

```
src/
├── App.jsx                # Main application component
├── App.css                # Global styles
├── main.jsx               # Application entry point
├── assets/
│   ├── components/        # Reusable components
│   │   ├── Footer/        # Footer component
│   │   ├── Header/        # Header with search functionality
│   │   ├── PokemonCard/   # Card component for each Pokémon
│   │   ├── PokemonDetail/ # Detailed view component
│   │   └── PokemonList/   # List component with pagination
│   ├── routes/            # Router configuration
│   ├── utils/             # Utility functions
│   │   ├── fetch.js       # API fetch functions
│   │   └── textFormat.js  # Text formatting utilities
│   └── views/             # Page components
│       ├── Detail/        # Pokémon detail page
│       ├── ErrorPage/     # Error page
│       ├── Home/          # Home page with Pokémon list
│       └── Type/          # Type-filtered Pokémon list
```

## 🌐 API

This application uses the [PokéAPI](https://pokeapi.co/) as its data source. The API is free to use and does not require authentication.

Key endpoints used:
- `GET https://pokeapi.co/api/v2/pokemon` - Get a list of Pokémon
- `GET https://pokeapi.co/api/v2/pokemon/{id or name}` - Get detailed information about a specific Pokémon
- `GET https://pokeapi.co/api/v2/type/{id or name}` - Get Pokémon of a specific type

## 🚀 Deployment

To build for production:

```bash
npm run build
# or
yarn build
```

This will create a `dist` folder with the compiled assets ready for deployment to any static web hosting service.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [PokéAPI](https://pokeapi.co/) for the Pokémon data
- Pokémon is © Nintendo, Game Freak, and The Pokémon Company
- This is a fan project and is not affiliated with the official Pokémon franchise
