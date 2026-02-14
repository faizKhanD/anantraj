# Anantraj Backend

Anantraj is a robust, high-performance backend system built with Node.js and TypeScript. It leverages Sequelize (PostgreSQL) and MongoDB for data management, providing a scalable architecture for complex data handling, real-time communications, and secure API services.

## 🚀 Tech Stack

- **Runtime**: Node.js
- **Language**: TypeScript
- **Framework**: Express.js
- **Database (Relational)**: PostgreSQL with Sequelize ORM
- **Database (NoSQL)**: MongoDB with Mongoose
- **API Documentation**: Swagger (OpenAPI)
- **Cloud Integration**: AWS S3 (for file storage), ImageKit
- **Real-time**: Socket.io
- **Security**: JWT, Passport.js, Helmet, Bcrypt, Express Rate Limit
- **Validation**: Joi, Express Validator
- **Logging**: Winston, Morgan
- **Utilities**: ExcelJS, XLSX, CSVtoJSON, Nodemailer

## 📁 Project Structure

```text
anantraj/
├── config/             # Database and environment configurations
├── dist/               # Compiled JavaScript files (after build)
├── logs/               # Application log files
├── migrations/         # Sequelize database migrations
├── seeders/            # Database seed data
├── src/                # Main source code
│   ├── config/         # App-specific configurations
│   ├── controllers/    # API request handlers
│   ├── interfaces/     # TypeScript interfaces and types
│   ├── middleware/     # Custom Express middlewares
│   ├── models/         # Sequelize and Mongoose database models
│   ├── routes/         # Express API route definitions
│   ├── utils/          # Helper functions and utilities
│   ├── validation/     # Request validation schemas (Joi/Express-validator)
│   └── server.ts       # Main entry point of the application
├── tsconfig.json       # TypeScript configuration
└── .env                # Environment variables (Sensitive!)
```

## 🛠️ Key Features

- **Multi-Database Support**: Efficiently uses PostgreSQL for structured relational data and MongoDB for flexible document storage.
- **Auto-generated Documentation**: Interactive API testing and documentation via Swagger UI.
- **Secure Authentication**: Robust JWT-based authentication system with Passport.js integration.
- **File Management**: Integrated AWS S3 and ImageKit support for high-availability file uploads and image transformation.
- **Real-time Updates**: Socket.io support for push notifications and live data sync.
- **Automated Workflows**: Database migrations and seeding handled via Sequelize CLI.
- **Excel/CSV Processing**: Built-in support for importing and exporting data in Excel and CSV formats.

## ⚙️ Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- PostgreSQL
- MongoDB
- Git

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd anantraj
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Environment Setup**:
   Create a `.env` file in the root directory and configure the necessary variables (DB credentials, AWS keys, etc.).

### Database Setup

Run the following commands to initialize your database:

```bash
# Run migrations
npm run migrate

# Seed initial data
npm run seed
```

### Running the Project

- **Development Mode** (with hot-reloading):
  ```bash
  npm run dev
  ```

- **Production Build**:
  ```bash
  npm run build
  npm start
  ```

## 📝 Available Scripts

- `npm run dev`: Starts the development server using `ts-node-dev`.
- `npm run build`: Compiles TypeScript files into the `dist` folder.
- `npm start`: Runs the compiled application from the `dist` folder.
- `npm run lint`: Perfroms linting checks using ESLint.
- `npm run migrate`: Executes all pending Sequelize migrations.
- `npm run seed`: Populates the database with seeders.
- `npm run deploy`: Automated deployment script (git pull, build, pm2 restart).

## 📄 API Documentation

Once the server is running, you can access the interactive Swagger documentation at:
`http://localhost:<PORT>/api-docs` (Exact port depends on your `.env` configuration).

---

**Author**: Faiz (react.faiyaz@gtftechnologies.com)
**License**: MIT
# anantraj
