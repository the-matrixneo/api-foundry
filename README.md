# API Foundry
## Quick start

Prerequisites
- Node.js 18+ (or the version your project requires)
- npm, yarn, or pnpm

Clone and install

1. Clone the repo

   git clone https://github.com/the-matrixneo/api-foundry.git
   cd api-foundry

2. Install dependencies

   npm install
   # or
   yarn install
   # or
   pnpm install

3. Create environment file

   Copy .env.example to .env and update values as needed.

4. Run in development mode

   npm run dev
   # or
   yarn dev
   # or
   pnpm dev

5. Open http://localhost:3000 (or the port configured in .env)

## Recommended project structure

This is a suggested layout — update to match the repository structure:
- src/
  - index.ts             # App entrypoint
  - server/              # Server config (express/fastify/koa)
  - routes/              # Route handlers
  - controllers/         # Business logic
  - services/            # Reusable services
  - middleware/          # Request middleware and error handlers
  - config/              # Configuration loader
  - tests/               # Unit and integration tests
- .env.example
- package.json
- tsconfig.json
- README.md

## Configuration
Use environment variables for configuration. A typical .env.example may contain:

PORT=3000
NODE_ENV=development
DATABASE_URL=
JWT_SECRET=

Load env vars early in the app (e.g. with dotenv) and validate required values.
