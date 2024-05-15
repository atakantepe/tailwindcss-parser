# TailwindCss Parser

This project is a utility for parsing Tailwind CSS files. It uses PostCSS to process CSS and outputs the results as JSON files.

This parser was used in the [TailwindCSS Cheat Sheet](https://github.com/atakantepe/tailwind-cheat-sheet) project.

...

## Scripts

This project includes the following npm scripts:

- `build:css`: This script runs postcss on `src/styles.css` and outputs the result to `src/assets/tailwind-output.css`.
- `parse`: This script runs a Node.js script (`src/parse-css.js`) that parses the CSS.
- `build-and-parse`: This script runs both `build:css` and `parse` in sequence.

## Usage

After cloning the repository and running `npm install`, you can generate the Tailwind CSS output and parse it into JSON files by running:

```bash
npm run build-and-parse
```

## Project Structure

tailwindcss-parser/
├── src/
│   ├── assets/
│   │   ├── (generated tailwindcss-output.css file will be here)
│   ├── data/
│   │   ├── (generated json files will be here)
│   ├── parse-css.js
│   ├── styles.css
├── node_modules/
├── package.json
├── postcss.config.js
└── tailwind.config.js

## Contributions

Contributions are always welcome! Here's how you can help:

- Report bugs
- Submit fixes and improvements via pull requests