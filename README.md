# Moishes Delivery App Backend Documentation

## Setup Instructions
1. **Clone the repository**:
   ```bash
   git clone https://github.com/<owner>/moishes-delivery-app-backend.git
   cd moishes-delivery-app-backend
   ```

2. **Install dependencies**:
   Ensure you have `Node.js` and `npm` installed. Run:
   ```bash
   npm install
   ```

3. **Configuration**:
   Create a `.env` file in the root directory based on the provided `.env.example`:
   ```bash
   cp .env.example .env
   ```
   Edit the `.env` file to set your environment variables.

4. **Run the application**:
   ```bash
   npm start
   ```

## Project Structure
```
moishes-delivery-app-backend/
│
├── src/
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   ├── utils/
│   └── index.js
│
├── tests/
│
├── .env.example
├── package.json
└── README.md
```

## API Endpoints Overview
### Authentication
- `POST /api/auth/login` - Login user.
- `POST /api/auth/register` - Register new user.

### Delivery Management
- `GET /api/deliveries` - Retrieve all deliveries.
- `POST /api/deliveries` - Create new delivery.
- `PUT /api/deliveries/:id` - Update delivery status.
- `DELETE /api/deliveries/:id` - Delete a delivery.

### User Management
- `GET /api/users` - Retrieve all users.
- `GET /api/users/:id` - Retrieve user by ID.

## Tech Stack
- **Node.js** - JavaScript runtime environment.
- **Express** - Web application framework.
- **MongoDB** - NoSQL database.
- **Mongoose** - ODM for MongoDB.
- **JWT** - Authentication method.
- **Mocha/Chai** - Testing suite.

---