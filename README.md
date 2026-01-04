# FoodieLocal

<div align="center">

[![GitHub stars](https://img.shields.io/github/stars/CipherSaber/FoodieLocal?style=for-the-badge&logo=github&logoColor=white)](https://github.com/CipherSaber/FoodieLocal/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/CipherSaber/FoodieLocal?style=for-the-badge&logo=github&logoColor=white)](https://github.com/CipherSaber/FoodieLocal/network)
[![GitHub issues](https://img.shields.io/github/issues/CipherSaber/FoodieLocal?style=for-the-badge&logo=github&logoColor=white)](https://github.com/CipherSaber/FoodieLocal/issues)
[![GitHub license](https://img.shields.io/github/license/CipherSaber/FoodieLocal?style=for-the-badge&logo=github&logoColor=white)](LICENSE)

**Connecting home chefs with nearby customers for fresh, home-cooked meal delivery.**

[Live Demo](https://ciphersaber.github.io/FoodieLocal/) 

</div>

## 📖 Overview

FoodieLocal is a full-stack web application designed to bridge the gap between talented home chefs and local customers seeking delicious, homemade meals. It empowers chefs to showcase their culinary creations and manage orders, while providing customers with a convenient platform to discover, order, and enjoy fresh, locally prepared food delivered right to their doorstep or available for pickup. The application aims to foster community connections through food, support local businesses, and offer a healthier, more personal alternative to conventional takeout options.

## ✨ Features

-   **🧑‍🍳 Chef & Customer Accounts:** Separate user roles with dedicated dashboards for managing profiles, meals, and orders.
-   **🍽️ Meal Management:** Chefs can easily add, edit, and remove meal listings with detailed descriptions, pricing, availability, and images.
-   **🔍 Advanced Meal Discovery:** Customers can browse, search, and filter meals by chef, cuisine type, dietary needs, and proximity.
-   **🛒 Seamless Ordering System:** Intuitive shopping cart functionality and a streamlined checkout process for customers.
-   **💳 Secure Payment Gateway:** Integrated secure online payment processing for hassle-free transactions.
-   **🚚 Order Tracking & Notifications:** Real-time updates for customers on their order status and management tools for chefs.
-   **⭐ Ratings & Reviews:** Customers can provide feedback on meals and chefs, building trust and community.
-   **📱 Responsive User Interface:** A beautiful and accessible design that works flawlessly across desktops, tablets, and mobile devices.
## 🛠️ Tech Stack

**Frontend:**
[![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=white)](https://react.dev/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)
[![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/)

**Backend:**
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)](https://nodejs.org/)
[![Express.js](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)](https://www.mongodb.com/)
[![Mongoose ODM](https://img.shields.io/badge/Mongoose-800000?style=for-the-badge&logo=mongoose&logoColor=white)](https://mongoosejs.com/)
[![JWT](https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=json-web-tokens&logoColor=white)](https://jwt.io/)
[![npm](https://img.shields.io/badge/npm-CB3837?style=for-the-badge&logo=npm&logoColor=white)](https://www.npmjs.com/)

**DevOps & Tools:**
[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)
[![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)](https://docs.github.com/en/actions)
[![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)](https://vercel.com/) <!-- For Frontend Deployment -->

## 🚀 Quick Start

Follow these steps to get FoodieLocal up and running on your local machine.

### Prerequisites
Before you begin, ensure you have the following installed:
-   **Node.js** (LTS version, e.g., 20.x or higher)
-   **npm** (comes with Node.js)
-   **MongoDB** (Community Server for local development, or access to a cloud instance like MongoDB Atlas)

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/CipherSaber/FoodieLocal.git
    cd FoodieLocal
    ```

2.  **Install Backend Dependencies**
    Navigate to the `backend` directory and install dependencies:
    ```bash
    cd backend
    npm install
    ```

3.  **Install Frontend Dependencies**
    Navigate to the `frontend` directory and install dependencies:
    ```bash
    cd ../frontend
    npm install
    ```

### Environment Setup

1.  **Backend Environment Variables**
    Create a `.env` file in the `backend` directory by copying the example:
    ```bash
    cp .env.example .env
    ```
    Open the `.env` file and configure the following variables:
    | Variable          | Description                                    | Default         | Required |
    |-------------------|------------------------------------------------|-----------------|----------|
    | `PORT`            | Port for the backend server to listen on.      | `5000`          | Yes      |
    | `MONGO_URI`       | Connection string for your MongoDB database.   | `mongodb://localhost:27017/foodielocal` | Yes      |
    | `JWT_SECRET`      | Secret key for signing JSON Web Tokens.        | (generate a strong, random string) | Yes |
    | `PAYMENT_GATEWAY_API_KEY` | API key for your chosen payment gateway. |                 | No       |
    | `GEOLOCATION_API_KEY` | API key for geolocation services.            |                 | No       |

2.  **Frontend Environment Variables**
    Create a `.env` file in the `frontend` directory by copying the example:
    ```bash
    cp .env.example .env
    ```
    Open the `.env` file and configure the following variables:
    | Variable          | Description                                    | Default         | Required |
    |-------------------|------------------------------------------------|-----------------|----------|
    | `VITE_API_BASE_URL` | Base URL of your backend API.                  | `http://localhost:5000/api` | Yes |
    | `VITE_GEOLOCATION_API_KEY` | API key for geolocation services (client-side). |                 | No       |

### Database Setup

Ensure your MongoDB instance is running. If you're using a local MongoDB server, start it. No specific migration commands are typically needed for Mongoose with MongoDB, as schemas are applied on connection.

### Start Development Servers

1.  **Start Backend Server**
    In the `backend` directory:
    ```bash
    npm run dev
    ```
    The backend server will typically start on `http://localhost:5000`.

2.  **Start Frontend Development Server**
    In a new terminal, navigate to the `frontend` directory:
    ```bash
    npm run dev
    ```
    The frontend application will typically start on `http://localhost:3000` (or another available port).

### Open your browser
Visit `http://localhost:3000` (or the port indicated by your frontend server) in your web browser.

## 📁 Project Structure

```
FoodieLocal/
├── .vscode/                 # VS Code configurations
├── backend/                 # Node.js Express API
│   ├── src/                 # Backend source code
│   │   ├── config/          # Environment and database configuration
│   │   ├── controllers/     # Route handlers
│   │   ├── middleware/      # Authentication, error handling
│   │   ├── models/          # Mongoose schemas for data
│   │   ├── routes/          # API endpoint definitions
│   │   └── server.js        # Main backend entry point
│   ├── .env.example         # Template for environment variables
│   ├── package.json         # Backend dependencies & scripts
│   └── (node_modules/)
├── frontend/                # React.js Application
│   ├── public/              # Static assets (index.html, favicon)
│   ├── src/                 # Frontend source code
│   │   ├── api/             # API service calls
│   │   ├── assets/          # Images, icons
│   │   ├── components/      # Reusable UI components
│   │   ├── hooks/           # Custom React hooks
│   │   ├── pages/           # Main application pages/views
│   │   ├── contexts/        # React Context API for global state
│   │   ├── styles/          # Global styles, Tailwind config
│   │   └── App.jsx          # Main application component
│   ├── .env.example         # Template for environment variables
│   ├── package.json         # Frontend dependencies & scripts
│   ├── tailwind.config.js   # Tailwind CSS configuration
│   ├── vite.config.js       # Vite build configuration
│   └── (node_modules/)
├── README.md                # Project documentation
└── .gitignore               # Files/directories to ignore
```

## ⚙️ Configuration

### Environment Variables
Configure `.env` files in both `backend` and `frontend` directories as described in the [Environment Setup](#environment-setup) section.

### Backend Configuration
*   `backend/src/config/index.js` (inferred): Contains database connection logic, JWT settings, etc.
*   `backend/src/middleware/auth.js` (inferred): JWT verification and role-based access control.

### Frontend Configuration
*   `frontend/tailwind.config.js` (inferred): Customization for Tailwind CSS.
*   `frontend/vite.config.js` (inferred): Frontend build and development server settings.

## 🔧 Development

### Available Scripts

#### Backend (`backend/package.json`)
| Command           | Description                                    |
|-------------------|------------------------------------------------|
| `npm install`     | Installs backend dependencies.                 |
| `npm run dev`     | Starts the backend server in development mode. |
| `npm start`       | Starts the backend server (for production).    |
| `npm run test`    | Runs backend tests.                            | <!-- TODO: Verify test command -->

#### Frontend (`frontend/package.json`)
| Command           | Description                                    |
|-------------------|------------------------------------------------|
| `npm install`     | Installs frontend dependencies.                |
| `npm run dev`     | Starts the frontend development server.        |
| `npm run build`   | Builds the frontend for production.            |
| `npm run lint`    | Lints frontend source code.                    |
| `npm run preview` | Serves the production build locally.           |
| `npm run test`    | Runs frontend tests.                           | <!-- TODO: Verify test command -->

### Development Workflow
To run the full application locally:
1.  Open two separate terminal windows.
2.  In the first terminal, navigate to the `backend` directory and run `npm run dev`.
3.  In the second terminal, navigate to the `frontend` directory and run `npm run dev`.
4.  Ensure your MongoDB database is running and accessible.
   
### Running Tests
To run all tests:
```bash
# For backend
cd backend
npm run test

# For frontend
cd frontend
npm run test
```

## 🚀 Deployment

FoodieLocal is a full-stack application, requiring separate deployment strategies for its frontend and backend components.

### Production Build
To create a production-ready build of the frontend:
```bash
cd frontend
npm run build
```
This will generate optimized static assets in the `dist` (or `build`) directory.

### Deployment Options

-   **Frontend (Static Hosting):**
    -   **Vercel / Netlify:** Ideal for deploying the `frontend/dist` (or `frontend/build`) folder as a static site. Configure environment variables for API communication.
    -   **GitHub Pages:** As indicated by the `homepage` URL, this is currently used for a static deployment, likely for the frontend only.

-   **Backend (Server Hosting):**
    -   **Render / Heroku:** Cloud platforms that provide easy deployment for Node.js applications and connect to MongoDB Atlas for the database.
    -   **AWS / GCP / Azure:** For more scalable and robust deployments, services like AWS EC2/ECS, GCP Cloud Run/App Engine, or Azure App Service can host the Node.js backend.
    -   **Docker:** A `Dockerfile` (if present in `backend/` or root) can be used to containerize the backend for deployment to any container orchestration platform (e.g., Kubernetes).

## 📚 API Reference

The backend provides a RESTful API for managing users, chefs, meals, orders, and payments.

### Authentication
The API uses **JSON Web Tokens (JWT)** for authentication.
-   Users register (`POST /api/auth/register`) and login (`POST /api/auth/login`) to receive a JWT.
-   This token should be included in the `Authorization` header of subsequent requests as a Bearer token: `Authorization: Bearer <token>`.

### Endpoints
Below is a high-level overview of the API structure. For detailed schema and request/response examples, please refer to the dedicated API documentation. <!-- TODO: Link to actual API docs -->

| Method | Endpoint                    | Description                                       | Authentication | Roles       |
|:-------|:----------------------------|:--------------------------------------------------|:---------------|:------------|
| `POST` | `/api/auth/register`        | Register a new user (customer or chef).           | None           | All         |
| `POST` | `/api/auth/login`           | Log in an existing user.                          | None           | All         |
| `GET`  | `/api/users/profile`        | Get current user's profile.                       | Required       | All         |
| `PUT`  | `/api/users/profile`        | Update current user's profile.                    | Required       | All         |
| `GET`  | `/api/chefs`                | Get all chef profiles.                            | Optional       | All         |
| `GET`  | `/api/chefs/:id`            | Get a specific chef's profile.                    | Optional       | All         |
| `POST` | `/api/meals`                | Create a new meal offering.                       | Required       | Chef        |
| `GET`  | `/api/meals`                | Get all meal offerings (with filters).            | Optional       | All         |
| `GET`  | `/api/meals/:id`            | Get a specific meal offering.                     | Optional       | All         |
| `PUT`  | `/api/meals/:id`            | Update a meal offering.                           | Required       | Chef        |
| `DELETE`| `/api/meals/:id`           | Delete a meal offering.                           | Required       | Chef        |
| `POST` | `/api/orders`               | Place a new order.                                | Required       | Customer    |
| `GET`  | `/api/orders/me`            | Get current user's orders.                        | Required       | All         |
| `GET`  | `/api/orders/chef`          | Get orders for the current chef.                  | Required       | Chef        |
| `PUT`  | `/api/orders/:id/status`    | Update order status (e.g., "preparing", "ready"). | Required       | Chef        |
| `POST` | `/api/payments/process`     | Process payment for an order.                     | Required       | Customer    |

## 🤝 Contributing

We welcome contributions to FoodieLocal! If you're interested in improving the project, please follow these steps:

1.  Fork the repository.
2.  Create a new branch (`git checkout -b feature/your-feature-name`).
3.  Make your changes and ensure they adhere to the project's coding standards.
4.  Write clear, concise commit messages.
5.  Push your branch (`git push origin feature/your-feature-name`).
6.  Open a Pull Request with a detailed description of your changes.

### Development Setup for Contributors
The development setup is the same as described in the [Quick Start](#quick-start) section. Ensure both frontend and backend are running concurrently.

## 📄 License

This project is licensed under the [MIT License](LICENSE) <!-- TODO: Add actual license file (LICENSE) --> - see the LICENSE file for details.

## 🙏 Acknowledgments

-   Inspired by the growing demand for local and homemade food options.
-   Built with the amazing open-source community's tools and libraries.
-   Special thanks to all contributors who help make FoodieLocal better.

## 📞 Support & Contact

If you have any questions, suggestions, or encounter issues, please feel free to reach out:
-   🐛 Issues: [GitHub Issues](https://github.com/CipherSaber/FoodieLocal/issues)
-   💬 Discussions: [GitHub Discussions](https://github.com/CipherSaber/FoodieLocal/discussions) <!-- TODO: Enable GitHub Discussions if not already -->

---
## Screenshot
<img width="1864" height="1017" alt="Fl" src="https://github.com/user-attachments/assets/210854a8-0adf-4dd6-8289-d5e153b07fec" />

<div align="center">

**⭐ Star this repo if you find it helpful!**

Made with ❤️ by [CipherSaber](https://github.com/CipherSaber)

</div>
```

