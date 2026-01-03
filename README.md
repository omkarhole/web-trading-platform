# Web Trading Platform  [Link](https://zerodha-c7dx.onrender.com)

A real-time web trading platform that simulates trading activity using WebSockets. Built with the MERN stack (MongoDB, Express, React, Node.js) and Socket.io for live communication.

## Features

- 📈 Real-time stock data updates using Socket.IO
- 👤 User authentication and session management.
- 🧾 Order placement and history tracking
- 🗃️ MongoDB for persistent storage
- 🎨 React-based responsive UI with Vite for fast builds

## Tech Stack

- **Frontend**: React, Vite, TailwindCSS
- **Backend**: Node.js, Express, Socket.IO, MongoDB
- **Other Tools**: Mongoose, JWT, dotenv

## Installation

1. Clone the repository
```bash
git clone https://github.com/omkarhole/web-trading-platform.git
cd web-trading-platform
```

2. Install backend dependencies
```bash
npm install
```

3. Install frontend dependencies
```bash
cd client
npm install
cd ..
```

4. Create environment file
```bash
cp .env.example .env
```

5. Configure your environment variables in `.env`:
```
PORT=5000
MONGODB_URI=mongodb://localhost:27017/trading-platform
JWT_SECRET=your-jwt-secret-key
NODE_ENV=development
```

6. Make sure MongoDB is running on your system

7. Start the development servers

Backend server:
```bash
npm run dev
```

Frontend server (in a new terminal):
```bash
cd client
npm run dev
```

8. Open your browser and navigate to `http://localhost:3000`

## API Endpoints

### Authentication
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - User login
- `GET /api/auth/profile` - Get user profile

### Trading
- `GET /api/stocks` - Get all stocks
- `GET /api/stocks/:symbol` - Get specific stock data
- `POST /api/orders` - Place new order
- `GET /api/orders` - Get user orders
- `DELETE /api/orders/:id` - Cancel order

### Portfolio
- `GET /api/portfolio` - Get user portfolio
- `GET /api/portfolio/history` - Get trading history

## Usage

1. Register a new account or login with existing credentials
2. View real-time stock prices on the dashboard
3. Place buy/sell orders using the trading interface
4. Monitor your portfolio and trading history
5. Receive real-time updates via WebSocket connections

## Project Structure

```
web-trading-platform/
├── client/                 # React frontend
│   ├── src/
│   ├── public/
│   └── package.json
├── server/                 # Express backend
│   ├── models/
│   ├── routes/
│   ├── middleware/
│   └── server.js
├── .env.example
├── package.json
└── README.md
```

## Scripts

- `npm run dev` - Start backend development server
- `npm run start` - Start backend production server
- `npm test` - Run tests
- `npm run build` - Build frontend for production

## Contributing

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

Omkar Hole - omkarhole314@gmail.com

Project Link: [github](https://github.com/omkarhole/web-trading-platform)
