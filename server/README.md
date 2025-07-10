# NLW Agents

A simple Fastify + Drizzle ORM backend project for managing rooms, using PostgreSQL with vector extension support.

## Tech Stack

- **Node.js** (TypeScript)
- **Fastify**: Web server framework
- **Zod**: Schema validation
- **Drizzle ORM**: Type-safe SQL ORM
- **PostgreSQL**: Database (with `pgvector` extension)
- **Docker**: For local database setup
- **Biome**: Code formatting and linting

## Project Structure & Patterns

- **src/server.ts**: Main entry point, sets up Fastify server and routes.
- **src/db/schema/**: Database schema definitions (Drizzle ORM).
- **src/db/migrations/**: Database migration files.
- **src/db/http/routes/**: HTTP route handlers (REST API pattern).
- **src/env.ts**: Environment variable validation using Zod.

## Setup & Configuration

### Prerequisites

- Node.js (v18+ recommended)
- Docker (for local PostgreSQL)

### 1. Install dependencies

```bash
npm install
```

### 2. Configure environment

Create a `.env` file in the project root with:

```
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/agents
```

### 3. Start PostgreSQL with Docker

```bash
docker-compose up -d
```

This will start a PostgreSQL instance with the `pgvector` extension enabled.

### 4. Run database migrations

```bash
npx drizzle-kit migrate
```

### 5. (Optional) Seed the database

```bash
npm run db:seed
```

### 6. Start the server

```bash
npm run dev
```

The API will be available at `http://localhost:3333`.
