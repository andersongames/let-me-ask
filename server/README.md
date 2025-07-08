# 🤖 NLW Agents

Project developed during a 🚀 Rocketseat event using modern technologies to create an API integrated with AI.

## 🧰 Technologies

- **Node.js with native TypeScript** (experimental strip types)
- **Fastify** – Fast and efficient web framework
- **PostgreSQL with pgvector extension** for vector storage
- **Drizzle ORM** – Type-safe database operations
- **Zod** – Schema validation
- **Docker** – Containerized database setup
- **Biome** – Code linting and formatting

## 🧱 Architecture

The project follows a modular architecture with:

- Separation of concerns between routes, schemas, and database connection
- Schema validation with Zod for type safety
- Type-safe ORM with Drizzle for database operations
- Centralized environment variable validation

## ⚙️ Setup and Configuration

### ✅ Prerequisites

- Node.js (version with support for `--experimental-strip-types`)
- Docker and Docker Compose

### 1. Clone the repository

```bash
git clone <repository-url>
cd server
```

### 2. Set up the database

```bash
docker-compose up -d
```

### 3. Configure environment variables

Create a `.env` file in the root of the project (`/server`):

```
PORT=3333
DATABASE_URL="postgresql://docker:docker@localhost:5432/letmeask"
```

### 4. Install dependencies

```bash
npm install
```

### 5. Run database migrations

```bash
npx drizzle-kit migrate
```

### 6. (Optional) Seed the database with example data

```bash
npm run db:seed
```

### 7. Run the project

**Development:**

```bash
npm run dev
```

**Production:**

```bash
npm run start
```

## 📜 Available Scripts

- `npm run dev` – Runs the server in development mode with hot reload 🔁
- `npm run start` – Runs the server in production mode 🚀
- `npm run db:seed` – Populates the database with sample data 🌱

## 🌐 Endpoints

The API will be available at `http://localhost:3333`

- `GET /health` – 💓 Application health check
- `GET /rooms` – 🏠 List available rooms