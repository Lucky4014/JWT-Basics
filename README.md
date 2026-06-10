JWT Authentication (MERN Stack)

## What I Built
Secure Signup/Login system using JWT tokens and bcrypt password hashing.

## Tech Used
- Node.js, Express.js
- MongoDB + Mongoose
- jsonwebtoken
- bcryptjs
- dotenv

## Folder Structure
server/
├── middleware/verifyToken.js
├── models/User.js
├── routes/auth.js
├── .env
└── server.js

## API Routes
| Method | Route | Description |
|--------|-------|-------------|
| POST | /api/auth/signup | Register new user |
| POST | /api/auth/login | Login + get JWT token |

## How to Run
1. npm install
2. Add .env file with MONGO_URI and JWT_SECRET
3. node server.js

## How JWT Works
When user logs in → server generates a token with user data (payload)
→ client stores token → sends it with every protected request.
