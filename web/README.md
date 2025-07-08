# 🌐 NLW Agents - Frontend

Project developed during a 🚀 Rocketseat event to demonstrate the use of AI agents on the web.

## 🧰 Technologies

- **React** – Library for building user interfaces
- **TypeScript** – JavaScript superset with static typing
- **Vite** – Fast build tool and development server
- **Tailwind CSS** – Utility-first CSS framework
- **React Router DOM** – Routing library for React
- **TanStack React Query** – Server state management and caching
- **Radix UI** – Accessible primitive components
- **shadcn/ui** – Component system
- **Lucide React** – Icon library

## 🧱 Design Patterns

- **Component-based Architecture** – Modular UI with reusable React components
- **File-based Routing** – Routing based on file structure using React Router
- **Server State Management** – Managed via React Query
- **Variant-based Components** – Using CVA (Class Variance Authority)
- **Composition Patterns** – With Radix Slot for flexible components
- **Path Aliasing** – Aliases like `@/` point to `src/`

## ⚙️ Project Setup

### ✅ Prerequisites

- Node.js (version 18 or above)
- npm or yarn

### Installation

### 1. Clone the repository

```bash
git clone <repository-url>
cd web
```

### 2. Install dependencies

```bash
npm install
```

### 3. Run development server

```bash
npm run dev
```

### 4. Open the app at: [http://localhost:5173](http://localhost:5173)

## 📜 Available Scripts

- `npm run dev` – Starts the development server
- `npm run build` – Builds the app for production
- `npm run preview` – Previews the production build

## 🔗 Backend Dependency

This project consumes an API that must be running on port `3333`. Make sure the backend is properly configured and running before starting the frontend.

## 🗂️ Project Structure

```
src/
├── components/ui     # UI components
├── pages/            # Application pages
├── lib/              # Utilities and configs
└── app.tsx           # Root component
```