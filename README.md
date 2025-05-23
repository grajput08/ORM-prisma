# ORM-prisma

A Node.js project using Prisma ORM for database management.

## Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- PostgreSQL (or your preferred database)

## Installation

1. Clone the repository:

```bash
git clone <repository-url>
cd orm-prisma
```

2. Install dependencies:

```bash
npm install
# or
yarn install
```

3. Set up your environment variables:
   Create a `.env` file in the root directory and add your database connection URL:

```
DATABASE_URL="postgresql://username:password@localhost:5432/database_name"
```

4. Initialize Prisma:

```bash
npx prisma init
```

5. Generate Prisma Client:

```bash
npx prisma generate
```

6. Run database migrations:

```bash
npx prisma migrate dev
```

## Project Structure

```
orm-prisma/
├── prisma/
│   ├── schema.prisma    # Database schema definition
│   └── migrations/      # Database migrations
├── src/
│   ├── index.ts       # index file
├── .env               # Environment variables
└── package.json       # Project dependencies
```

## Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build the project
- `npm start` - Start production server
- `npx prisma migrate dev` - Create and apply database migrations
- `npx prisma generate` - Generate Prisma Client

## Database Management

### Creating Migrations

When you make changes to your schema:

```bash
npx prisma migrate dev --name <migration-name>
```

### Resetting Database

To reset your database (CAUTION: This will delete all data):

```bash
npx prisma migrate reset
```

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For support, please open an issue in the GitHub repository or contact the maintainers.
