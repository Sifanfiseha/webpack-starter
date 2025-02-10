# Webpack Starter

A simple Webpack starter setup with Babel, CSS extraction, and HTML template support.

## Features

- Webpack for bundling JavaScript and CSS files
- Babel for transpiling modern JavaScript
- MiniCssExtractPlugin for extracting CSS into separate files
- HtmlWebpackPlugin for generating an HTML file
- Webpack DevServer for live reloading

## Installation

Clone the repository and install dependencies:

```sh
npm install
```

## Usage

### Development Mode

Run Webpack in development mode with hot reloading:

```sh
npm start
```

### Production Build

Generate a production-ready build:

```sh
npm run build
```

## Project Structure

```
/project-root
│── dist/                # Output directory
│── src/                 # Source files
│   ├── index.js         # Main JavaScript file
│   ├── styles.css       # Main CSS file
│   ├── index.html       # HTML template
│── webpack.config.js    # Webpack configuration
│── package.json         # Project dependencies
│── .babelrc             # Babel configuration
```

## Webpack Configuration

### Entry and Output

- Entry file: `src/index.js`
- Output file: `dist/bundle.js`

### Loaders

- **CSS Loader:** Handles CSS files (`.css`)
- **Babel Loader:** Transpiles ES6+ JavaScript (`.js`)

### Plugins

- **HtmlWebpackPlugin:** Generates an `index.html` file from `src/index.html`
- **MiniCssExtractPlugin:** Extracts CSS into separate files

### DevServer

- Serves files from `dist/`
- Runs on `localhost:3000`
- Supports hot module replacement (HMR)

## Dependencies

### Dev Dependencies

- `webpack`, `webpack-cli`, `webpack-dev-server`
- `babel-loader`, `@babel/core`, `@babel/preset-env`
- `css-loader`, `mini-css-extract-plugin`, `style-loader`
- `html-webpack-plugin`
