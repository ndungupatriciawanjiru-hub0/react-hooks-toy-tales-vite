# Toy Tales

A React single-page app that connects to a `json-server` backend to manage a toy collection with full CRUD functionality.

## Features

- **View toys** — fetches all toys from the backend and displays them as cards on page load.
- **Add a toy** — a form lets you create a new toy (name + image URL), which is saved to the backend and immediately added to the page.
- **Like a toy** — clicking "Like" increases a toy's like count, both on the server and on the page.
- **Donate a toy** — clicking "Donate to GoodWill" deletes the toy from the backend and removes its card from the page.

## Setup

1. Clone this repo and install dependencies:
```bash
   npm install
```
2. Start the backend (json-server on port 3001):
```bash
   npm run server
```
3. In a separate terminal, start the React app (port 3000):
```bash
   npm run dev
```
4. To run the test suite:
```bash
   npm run test -- --run
```

## Tech stack

React, Vite, json-server, Vitest, React Testing Library.

## Known limitations

Toy data resets to `db.json`'s contents if the file is manually restored; there's no persistent database beyond the local JSON file.

## Screenshot

_Add a screenshot of the app here, e.g._
![Toy Tales screenshot](./screenshot.png)