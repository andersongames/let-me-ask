# 🤖 NLW Agents - Backend

Project developed during a 🚀 Rocketseat event using modern technologies to create an API integrated with AI agents.

## 🧰 Technologies

- **Node.js with native TypeScript** – JavaScript superset with experimental `--experimental-strip-types` support
- **Fastify** – Fast and efficient web framework for building APIs
- **PostgreSQL** – Relational database with the **pgvector** extension for vector embeddings
- **Drizzle ORM** – Type-safe, lightweight ORM for database operations
- **Zod** – Runtime schema validation and static type inference
- **Docker** – Containerized setup for running the database locally
- **Biome** – All-in-one tool for linting, formatting, and code analysis
- **Google Gemini** – AI model used for generating responses and processing content via API integration

## 🧱 Architecture

The project follows a modular and scalable architecture with:

- Clear separation of concerns between routes, schemas, controllers, and database layers
- Schema validation with **Zod** for type-safe API input handling
- Type-safe database operations using **Drizzle ORM**
- Centralized configuration of environment variables for consistency and security

## ⚙️ Setup and Configuration

### ✅ Prerequisites

- Node.js (version 18+ with support for `--experimental-strip-types`)
- Docker & Docker Compose

### 🚀 Getting Started

1. Clone the repository:

```bash
git clone <repository-url>
cd server
```

2. Start the database container:

```bash
docker-compose up -d
```

3. Create a `.env` file in the root of the `/server` folder:

```
PORT=3333
DATABASE_URL="postgresql://docker:docker@localhost:5432/letmeask"
GEMINI_API_KEY=[your-gemini-API-key]
```

4. Install project dependencies:

```bash
npm install
```

5. Run database migrations:

```bash
npm run db:migrate
```

6. (Optional) Seed the database with sample data:

```bash
npm run db:seed
```

7. Start the development server:

```bash
npm run dev
```

To run in production mode:

```bash
npm run start
```

## 📜 Available Scripts

- `npm run dev` – Starts the server in development mode with hot reload 🔁
- `npm run start` – Runs the server in production mode 🚀
- `npm run db:generate` – Generates SQL migration files based on schema changes
- `npm run db:migrate` – Runs the database migrations
- `npm run db:seed` – Populates the database with sample data 🌱

## 🌐 API Endpoints

Base URL: `http://localhost:3333`

- `GET /health` – 💓 Application health check
- `GET /rooms` – 🏠 Lists all available rooms
- `GET /rooms/:roomId/questions` – ❓ Retrieves all questions for a specific room
- `POST /rooms/:roomId/questions` – ✍️ Submits a new question to a specific room
- `POST /rooms` – ➕ Creates a new room
- `POST /rooms/:roomId/audio` – 🎙️ Uploads an audio file to be transcribed and processed via AI

## 🛠️ Useful Commands

- Generate migrations based on schema changes:
  ```bash
  npx drizzle-kit generate
  ```

- Apply migrations to the database:
  ```bash
  npx drizzle-kit migrate
  ```

- Open the Drizzle Studio interface:
  ```bash
  npx drizzle-kit studio
  ```