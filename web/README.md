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
- **Shadcn/ui** – Component system for building consistent UIs
- **Lucide React** – Icon library
- **Day.js** – Lightweight library for date manipulation and formatting
- **react-hook-form** – Performant, flexible form management library
- **Zod** – Type-safe schema validation for form inputs and API integration
- **Biome** – Tool for code formatting, linting, and static analysis

## 🧱 Design Patterns

- **Component-based Architecture** – Modular UI built with reusable React components
- **File-based Routing** – Routing system based on file structure using React Router
- **Server State Management** – Managed via React Query for async state and caching
- **Variant-based Components** – Styled components using Class Variance Authority (CVA)
- **Composition Patterns** – Slot-based component composition using Radix
- **Path Aliasing** – Path aliases like `@/` point to the `src/` folder

## ⚙️ Project Setup

### ✅ Prerequisites

- Node.js (version 18 or above)
- npm or yarn

### 🚀 Installation

1. Clone the repository

```bash
git clone <repository-url>
cd web
```

2. Install dependencies

```bash
npm install
```

3. Run development server

```bash
npm run dev
```

4. Open the application at: [http://localhost:5173](http://localhost:5173)

## 📜 Available Scripts

- `npm run dev` – Starts the development server 🚧
- `npm run build` – Builds the application for production 🏗️
- `npm run preview` – Previews the production build 🔍

## 🔗 Backend Dependency

This project consumes an API that must be running on port `3333`. Make sure the backend is properly configured and running before starting the frontend.

## 🗂️ Project Structure

```
src/
├── components/ui     # UI components
├── pages/            # Application pages
├── lib/              # Utilities and configurations
└── app.tsx           # Root component
```