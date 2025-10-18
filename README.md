# D.Watson Pharmacy Management System

A comprehensive pharmacy management system built with Node.js, Express, MongoDB, and vanilla JavaScript.

## 🚀 Features

- **Dashboard**: Real-time sales analytics and statistics
- **Inventory Management**: Product tracking with low stock alerts
- **Sales Management**: Complete POS system with invoice generation
- **Multi-Branch Support**: Manage multiple pharmacy branches
- **Category Management**: Organize products by categories
- **Reporting**: Sales reports and profit analysis

## 📋 Prerequisites

- Node.js (v14 or higher)
- MongoDB (v4.4 or higher)
- npm or yarn

## 🛠️ Installation

1. Clone the repository
```bash
git clone https://github.com/yourusername/pharmacy-management-system.git
cd pharmacy-management-system
```

2. Install dependencies
```bash
npm install
```

3. Create environment file
```bash
cp .env.example .env
```

4. Configure your `.env` file
```env
PORT=4000
MONGODB_URI=mongodb://127.0.0.1:27017/pharmacy_db
```

5. Start MongoDB service
```bash
# Windows
net start MongoDB

# macOS/Linux
sudo systemctl start mongod
```

6. Run the application
```bash
npm start
```

7. Open browser and navigate to

8. Deploy to Heroku

Option A (one-click - if you have a GitHub repo):

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy?template=https://github.com/yourusername/your-repo-name)

Option B (CLI):

```powershell
heroku login
heroku create your-app-name
heroku git:remote -a your-app-name
git push heroku main
heroku config:set MONGODB_URI="your_production_mongo_uri"
heroku ps:scale web=1
heroku open
```

Notes:
- The server listens on the port provided by Heroku via the `PORT` environment variable.
- You must set `MONGODB_URI` (or `MONGO_URL`) in Heroku config vars to point to your MongoDB Atlas cluster.
- The `Procfile` in the repo already points Heroku to start `node server/index.js`.

