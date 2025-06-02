# Credox Backend API

This is the backend API for the Credox trading platform.

## Setup

1. Install dependencies:
```
npm install
```

2. Start the server:
```
npm start
```

The server will run on port 5000 by default, or the port specified in the PORT environment variable.

## API Endpoints

### Authentication
- POST /api/auth/login - Login with email and password
- POST /api/auth/register - Register a new user

### Users
- GET /api/users - Get all users
- PUT /api/users/:id - Update a user

### Transactions
- GET /api/transactions - Get all transactions
- GET /api/transactions/user/:userId - Get transactions for a specific user
- POST /api/transactions - Create a new transaction

### Pending Transactions
- GET /api/pending-transactions - Get all pending transactions
- POST /api/pending-transactions - Create a new pending transaction
- PUT /api/pending-transactions/:id/approve - Approve a pending transaction
- PUT /api/pending-transactions/:id/reject - Reject a pending transaction

### KYC
- GET /api/pending-kyc - Get all pending KYC requests
- POST /api/pending-kyc - Create a new KYC request
- PUT /api/pending-kyc/:id/approve - Approve a KYC request
- PUT /api/pending-kyc/:id/reject - Reject a KYC request