# Top 10 Games

> A responsive, card-based ranking of ten favorite games.

[Live demo](https://lugarty.github.io/top-10-games/)

## Overview

Top 10 Games is a small static website that presents a personal ranking of ten games, with a short description for each entry. Selecting a card reveals its details.

## Features

- Ten ranked game cards
- Expandable descriptions
- Responsive layout
- Live deployment through GitHub Pages

## Tech Stack

- HTML5
- CSS3
- JavaScript
- Docker and GitHub Actions for local serving and automated checks

## Run Locally

Clone the repository and open `index.html` in a browser. For live reload during development, use the VS Code Live Server extension.

To serve the site with Docker:

```bash
docker build -t top-10-games .
docker run --rm -p 3000:3000 top-10-games
```

Then open `http://localhost:3000`.

## Validation

The GitHub Actions workflow runs HTMLHint, Stylelint, and ESLint on pushes and pull requests. These checks are currently advisory and do not block a successful workflow run.

## Project Structure

```text
.
├── .github/workflows/check-push.yml
├── figs/                 # Game images
├── Dockerfile
├── index.html
├── script.js
└── style.css
```

Lint configuration files are stored in the repository root.

## Project Status and License

This is a personal project and is not offered as a commercial product. No license has been specified.

## Author

[Anísio Oliveira (@Lugarty)](https://github.com/Lugarty)