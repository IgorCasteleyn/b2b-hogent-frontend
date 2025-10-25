# 2024 Frontend - Groep 14

Een moderne React-applicatie gebouwd met Vite, Chakra UI en React Router. Dit project is onderdeel van het SDP2-vak aan HOGENT.

## 📋 Project Beschrijving

Dit is een B2B frontend-applicatie met ondersteuning voor klanten en leveranciers. De applicatie biedt functionaliteiten voor:

- Authenticatie en autorisatie
- Productenbeheer
- Bestellingenbeheer
- Notificatiessysteem
- Gebruikersprofielen
- PDF-printing functionaliteit

## 🚀 Quick Start

### Installatie

```bash
yarn install
```

### Development Server

```bash
yarn dev
```

De applicatie wordt geopend op `http://localhost:5173` (Vite standaard poort).

### Build voor productie

```bash
yarn build
```

### Preview productie build

```bash
yarn preview
```

## 🧪 Testing

### Cypress E2E Tests

```bash
yarn test
```

Dit opent de Cypress Test Runner. Je kunt ook tests headless runnen met:

```bash
yarn cypress run
```

### Linting

```bash
yarn lint
```

## 📁 Project Structuur

```text
src/
├── main.jsx                 # Entry point
├── pages.jsx               # Route configuratie
├── main.css                # Globale stijlen
├── Componenten/            # React componenten
│   ├── Layout.jsx          # Root layout component
│   ├── Navbar.jsx          # Navigatiebalk
│   ├── Footer.jsx          # Footer component
│   ├── Login.jsx           # Login pagina
│   ├── Profiel.jsx         # Gebruikersprofiel
│   ├── PrivateRoute.jsx    # Protected routes
│   ├── contexts/           # React Context providers
│   │   ├── Auth.contexts.jsx
│   │   └── Notificatie.contexts.jsx
│   └── pages/              # Pagina componenten
│       ├── home/           # Homepagina met producten
│       ├── bestellingen/   # Bestellingenpagina's
│       └── notificaties/   # Notificatiepagina's
└── api/                    # API integratielaag
    └── index.js
```

## 🛠 Technologieën

- **React 18** - UI framework
- **Vite** - Build tool en dev server
- **Chakra UI** - Component library
- **React Router v6** - Client-side routing
- **Axios** - HTTP client
- **React Hook Form** - Form state management
- **React to Print** - PDF printing
- **Cypress** - E2E testing
- **ESLint** - Code linting

## 🔐 Testaccounts

### Klant Account

- **Gebruikersnaam:** klant2
- **Wachtwoord:** 12345678

### Leverancier Account

- **Gebruikersnaam:** leverancier2
- **Wachtwoord:** 12345678

### Alternatief Klant Account

- **Naam:** Klant1
- **Email:** lucaskatamadze.opleiding&#64;gmail.com
- **Wachtwoord:** SnoopG12345678

## 📝 NPM Scripts

| Script         | Beschrijving                |
| -------------- | --------------------------- |
| `yarn dev`     | Start de development server |
| `yarn build`   | Build voor productie        |
| `yarn preview` | Preview de production build |
| `yarn test`    | Open Cypress test runner    |
| `yarn lint`    | Voer ESLint linting uit     |

## 🔧 Configuratie

### Vite Config (`vite.config.js`)

- React plugin met SWC compiler voor snelle transpilatie

### Cypress Config (`cypress.config.js`)

- E2E test configuratie

## 📦 Dependencies

### Core

- `react`: ^18.2.0
- `react-dom`: ^18.2.0
- `react-router-dom`: ^6.22.2

### UI & Styling

- `@chakra-ui/react`: ^2.8.2
- `@chakra-ui/icons`: ^2.1.1
- `@emotion/react`: ^11.11.4
- `@emotion/styled`: ^11.11.0

### Icons & Utilities

- `@fortawesome/react-fontawesome`: ^0.2.0
- `react-floating-whatsapp`: ^5.0.8
- `react-to-print`: ^2.15.1
- `framer-motion`: ^11.0.6

### Forms & API

- `react-hook-form`: ^7.50.1
- `axios`: ^1.6.7
- `swr`: ^2.2.5
