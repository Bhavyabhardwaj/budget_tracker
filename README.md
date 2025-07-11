
# Budget Tracker.

## Overview
Budget Tracker is a simple and efficient application designed to help you manage your finances effectively. Follow the steps below to set up and deploy the project.

## Table of Contents
- [Installation](#installation)
- [Development Setup](#development-setup)
- [Production Deployment](#production-deployment)
- [Contributing](#contributing)

## Installation

### Clone the Repository
```sh
git clone https://github.com/Bhavyabhardwaj/budget_tracker.git
cd budget_tracker
```

### Install Dependencies
```sh
npm install
```

### Set Up Environment Variables
- Copy `.env.example` to `.env` and update it with your secrets:
```sh
cp .env.example .env
```

## Development Setup

### Prisma Migrations
- Run the following commands to set up Prisma:
```sh
npx prisma migrate dev --name <migration_name>
npx prisma generate
```

### Database Setup
- You can run PostgreSQL locally or use a hosted service such as:
  - [Neon](https://neon.tech)
  - [Avion](https://avion.io)

### Start Development Server
```sh
npm run dev
```

## Production Deployment

### Vercel Setup
- Go to the [Vercel Dashboard](https://vercel.com/dashboard) and navigate to **Storage** to set up a PostgreSQL database.
- Copy all required environment variables.

### Environment Variables
- Rename `.env.example` to `.env` and update it with your database secrets:
```sh
mv .env.example .env
```

- Add these secrets to Vercel's environment variables configuration.

### Deploy
- Deploy your application on Vercel by following the deployment steps in the Vercel dashboard.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.
