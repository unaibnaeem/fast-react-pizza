# Fast React Pizza 🍕

Fast React Pizza is a pizza-ordering web application built with React. Users can enter their name, browse the pizza menu, add pizzas to a cart, place an order, and look up an order using its order ID.

## Features

- **Get started with your name:** Enter a name to begin ordering.
- **Browse the menu:** View the available pizzas and their details.
- **Manage the cart:** See selected pizzas and manage the items before checkout.
- **Place an order:** Submit an order with the required customer and delivery details.
- **Search orders:** Look up an existing order using its order ID.
- **State management:** Use Redux Toolkit to manage application state, including cart-related state.

## Tech Stack

- React
- JavaScript
- CSS
- Redux Toolkit
- Vite

## Getting Started

### Prerequisites

Install [Node.js](https://nodejs.org/) (which includes npm).

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-REPOSITORY.git
cd YOUR-REPOSITORY
```

Replace the example repository URL and directory with your own.

### 2. Install dependencies

```bash
npm install
```

### 3. Configure the environment variable

Create a `.env` file in the project root, in the same directory as `package.json`:

```dotenv
VITE_API_URL=https://react-fast-pizza-api.onrender.com/api
```

This value is the API base URL used by the commonly used Fast React Pizza API. If your project connects to a different backend, set `VITE_API_URL` to that backend's base URL instead.

In the application code, read the variable with Vite's environment API, for example:

```js
const API_URL = import.meta.env.VITE_API_URL;
```

Update the existing API service or fetch calls to use `API_URL` instead of a hard-coded base URL. Check the project's existing API paths and keep them intact when replacing the base URL.

### 4. Start the development server

```bash
npm run dev
```

Open the local URL printed by Vite in your terminal.

## Environment Variable Notes

- Keep your local `.env` file out of Git by adding it to `.gitignore`.
- Commit an `.env.example` file with a safe placeholder so other developers know which variable to configure. For example:

  ```dotenv
  VITE_API_URL=https://your-api-base-url.example/api
  ```

- Restart the Vite development server after changing environment variables.
- `VITE_` variables are included in the client-side app bundle. Use this variable for a public API base URL, not for passwords, private tokens, or other secrets.

## Project Purpose

This project demonstrates a pizza-ordering flow with React, Redux Toolkit, and Vite, including menu browsing, cart management, order creation, and order lookup.
