# Certificate Generation Platform (Certi4U)

Built with:

- **Frontend:** React + Vite + Tailwind CSS
- **Backend:** Node.js + Express

## Table of Contents

- [Project Structure](#project-structure)
- [Installation](#installation)
- [Local Development](#local-development)
- [Build and Production](#build-and-production)

## Project Structure

```
.
├── client/            # React frontend (Vite + Tailwind CSS)
├── server/            # Express backend
├── package.json       # Root scripts for running and building the app
├── package-lock.json
├── .gitignore
└── README.md
```

## Installation

### 1. Clone the repository

```
git clone https://github.com/SaraByex/certificate-generation-platform.git
cd certificate-generation-platform
```

### 2. Install dependencies

Make sure you have [Node.js](https://nodejs.org/en) installed. Run the following command from the root folder:

```
npm run install-all
```

This runs:

- `npm install` for root
- `npm install` inside `/client`
- `npm install` inside `/server`

## Local Development

Run **frontend & backend** together from the root folder:

```
npm run dev
```

This uses **concurrently** to start both servers:

- `npm run dev --prefix client` → starts Vite dev server
- `npm run dev --prefix server` → starts Express server

Frontend is available at:

```
http://localhost:5173
```

Backend is available at:

```
http://localhost:3000
```

## Build and Production

### 1. Build the frontend from root:

```
npm run build
```

### 2. Start production server from root:

```
npm start
```

In production, **the Express app serves the built React app** from `/client/dist`. The app is accessible on your server URL, e.g.:

```
http://localhost:3000
```
# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
