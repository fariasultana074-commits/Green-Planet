Green Planet 🌱
Build Status License Version

Description
Green Planet is a comprehensive full-stack MERN (MongoDB, Express, React, Node.js) web application designed to foster a community around eco-friendly living and plant care. It provides a platform for users to buy and sell plants, donate or swap them with other enthusiasts, and engage with community-driven content through blogs and forums.

Green Planet was created to bridge the gap between local plant nurseries and eco-conscious individuals, reducing the carbon footprint of plant delivery while building a tight-knit community of green thumbs.

✨ Key Features
Robust Authentication & Authorization: Secure user registration, login, and JWT-based session management with role-based access control (User, Merchant, Admin).
Marketplace & E-commerce: Browse, filter, and search through a catalog of plants and eco-friendly products. Includes a complete shopping cart and checkout flow.
Merchant Dashboard: Users can become merchants, manage their own shops, and add/edit/delete their product listings.
Community Initiatives: Built-in functionalities to facilitate direct plant donations and community plant swaps.
Content & Engagement: A blogging platform for users to read and write about plant care, sustainability, and gardening tips.
Admin Panel: A dedicated interface for administrators to manage users, orders, and overall platform health.
🛠️ Tech Stack
Frontend:

React (v19) - UI Library
React Router DOM - Client-side routing
TailwindCSS - Utility-first styling
Axios - HTTP client for API requests
Backend:

Node.js & Express - Server environment and web framework
MongoDB & Mongoose - NoSQL Database & Object Data Modeling
JSON Web Tokens (JWT) & Bcrypt.js - Security & Authentication
Multer - Handling file / image uploads
🚀 Getting Started
Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

Prerequisites
Ensure you have the following installed on your local machine:

Node.js: (v16.x or higher)
npm: Node package manager
MongoDB: A running local instance or a MongoDB Atlas URI
Installation
Clone the repository

git clone <your-repository-url>
cd CSE470_Green_Planet
Install Backend Dependencies

cd backend
npm install
Install Frontend Dependencies

cd ../frontend
npm install
⚙️ Environment Variables
To run this project, you will need to add the following environment variables. Create a .env file in the respective directories.

Backend (/backend/.env)
Variable	Description	Example
NODE_ENV	Environment mode (development/production)	development
PORT	The port the backend server runs on	5000
MONGODB_URI / MONGO_URI	MongoDB connection string	mongodb://127.0.0.1:27017/greenplanet
JWT_SECRET	Secret key for signing JSON Web Tokens	your_super_secret_key_here
Frontend (/frontend/.env - optional for local dev)
Variable	Description	Example
REACT_APP_API_URL	Base URL for backend API requests	http://localhost:5000
💻 Usage
The project includes a convenient batch script to start both the frontend and backend servers simultaneously on Windows.

Start Both Servers (Windows)
Double-click the start-network.bat file in the root directory, or run it from the command line:

start-network.bat
Start Servers Manually (Cross-platform)
1. Start the Backend: Open a terminal and run:

cd backend
npm run dev
2. Start the Frontend: Open a new terminal window and run:

cd frontend
npm start
The frontend will typically be available at http://localhost:3000 and the backend API at http://localhost:5000.

📁 Project Structure
CSE470_Green_Planet/
├── backend/                  # Server-side code (Node.js/Express)
│   ├── config/               # Database and environment configurations
│   ├── controllers/          # API route logic
│   ├── middleware/           # Custom Express middleware (auth, errors)
│   ├── models/               # Mongoose database schemas
│   ├── routes/               # Express API routes
│   ├── scripts/              # Utility scripts
│   ├── utils/                # Helper functions (e.g., token generation)
│   └── index.js              # Entry point for backend
├── frontend/                 # Client-side code (React)
│   ├── public/               # Static assets
│   ├── src/                  # React source code
│   │   ├── components/       # Reusable UI components & pages
│   │   │   ├── auth/         # Authentication (Login, Signup, etc.)
│   │   │   ├── admin/        # Admin panel components
│   │   │   └── dashboard/    # Dashboard components
│   │   ├── config/           # Frontend configuration
│   │   ├── context/          # React Context providers (User, Cart)
│   │   ├── App.js            # Main application router
│   │   └── index.js          # Entry point for React
│   └── package.json          # Frontend dependencies
├── start-network.bat         # Script to run both servers (Windows)
└── README.md                 # Project documentation
🤝 Contributing
Contributions, issues, and feature requests are welcome!

Fork the Project
Create your Feature Branch (git checkout -b feature/AmazingFeature)
Commit your Changes (git commit -m 'Add some AmazingFeature')
Push to the Branch (git push origin feature/AmazingFeature)
Open a Pull Request
📄 License
This project is licensed under the MIT License.

Generated for Green Planet.
