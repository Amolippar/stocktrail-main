# StockTrail - Complete Project Documentation

## 1. Cover Page
**Project Name:** StockTrail
**Developer Name:** Amol (or Developer Name)
**Technology Stack:** Vue 3 (Vite), Node.js, Express, MongoDB, Tailwind CSS, Pinia
**Organization/Institute Name:** CDAC
**Project Duration:** Final Year Project Duration
**Version:** 1.0.0
**Date:** May 2026

---

## 4. Table of Contents
1. Cover Page
4. Table of Contents
5. Executive Summary
6. Project Introduction
7. Problem Statement
8. Goal of the Project
9. Project Scope
10. Objectives
11. Key Features
12. Technology Stack
13. System Architecture
14. Folder Structure Explanation
19. Authentication & Authorization Flow
20. Complete Workflow Explanation
25. Performance Optimization
26. Error Handling Strategy
27. UI/UX Documentation

---

## 5. Executive Summary
- **What the project does:** StockTrail is a full-stack financial dashboard designed to track stock portfolios, maintain user wallets, and securely handle KYC operations.
- **Main objective:** To provide users with an accessible, real-time platform to monitor financial data and perform simulated wallet transactions securely.
- **Technologies used:** MEVN Stack (MongoDB, Express.js, Vue 3, Node.js), Pinia for state management, and Tailwind CSS for styling.
- **Expected outcomes:** Delivery of a robust, scalable, and ATS-friendly fintech platform that meets modern industry standards for security and user experience.

---

## 6. Project Introduction
- **Project overview:** StockTrail is a secure web application that bridges the gap between complicated professional trading software and simple retail finance trackers.
- **Background:** The need arose from the complexity of managing multiple financial wallets and tracking KYC status across different platforms.
- **Business domain:** Financial Technology (FinTech).
- **Industry relevance:** With the surge in retail investors, platforms that simplify portfolio tracking are highly relevant in the modern tech landscape.
- **Why the project was created:** To demonstrate full-stack proficiency by solving the real-world problem of fragmented financial tracking for everyday users.

---

## 7. Problem Statement
- **Real-world problem solved:** Retail investors often struggle with disorganized financial tracking across disjointed applications.
- **Existing system limitations:** Existing solutions are either too complex (aimed at professional traders) or lack features like integrated wallet balance tracking and strict KYC enforcement.
- **Challenges faced by users:** Lack of a single dashboard to view wallet balances, transaction histories, and identity verification status.
- **Why this solution is important:** It centralizes essential financial tracking mechanisms into one beginner-friendly, secure, and intuitive dashboard.

---

## 8. Goal of the Project
- **Main goal:** To develop a functional, full-stack fintech tracking application.
- **Technical goals:** Implement secure REST APIs, establish a robust JWT authentication flow, and utilize the Vue 3 Composition API with Pinia for seamless reactivity.
- **Business goals:** Provide a clear, data-driven dashboard that accurately reflects a user's simulated financial state.
- **User goals:** Enable users to easily register, verify their KYC, and monitor their wallet with zero friction.
- **Security goals:** Ensure all endpoints are protected, passwords are cryptographically hashed, and sensitive data is restricted based on authorization tokens.
- **Performance goals:** Achieve fast UI load times via Vite bundling and optimize database queries using Mongoose indexing.

---

## 9. Project Scope
- **Current scope:** User authentication, JWT-based session management, wallet balance tracking, transaction history logging, and KYC status handling.
- **User scope:** Retail users requiring a centralized financial tracker.
- **Functional scope:** Registration, Login, Dashboard Visualization, KYC Upload, Wallet Management.
- **Technical scope:** Frontend SPA (Single Page Application) backed by a Node.js API and NoSQL database.
- **Operational scope:** Runs on modern web browsers and can be hosted on standard cloud platforms.
- **Scalability scope:** The Node.js event-driven architecture and stateless JWT auth allow the backend to scale horizontally easily.
- **Limitations of the project:** The project simulates wallet transactions and does not currently connect to real-world bank APIs or execute live stock trades.
- **Out-of-scope features:** High-frequency live trading execution, AI-based stock predictions, and real-money payment gateways.

---

## 10. Objectives
- **Primary objectives:** Deliver a fully functional MEVN stack application that correctly manages relational data (Users, Wallets, KYC).
- **Secondary objectives:** Implement an intuitive, responsive UI using Tailwind CSS and ApexCharts.
- **Functional objectives:** Ensure the wallet balances update correctly and KYC status accurately restricts or allows user actions.
- **Non-functional objectives:** Maintain high code quality, follow RESTful design principles, and ensure the UI is fully accessible and responsive.

---

## 11. Key Features
- **Feature Name:** Secure Authentication
  - **Description:** JWT-based login and registration system with hashed passwords.
  - **Benefits:** Prevents unauthorized access and protects user data.
  - **User impact:** Users feel secure knowing their financial data is protected.
- **Feature Name:** Wallet Management Dashboard
  - **Description:** A visual dashboard tracking current balances and transaction histories.
  - **Benefits:** Centralized view of financial standing.
  - **User impact:** Eliminates the need to manually track balances on spreadsheets.
- **Feature Name:** KYC Verification Workflow
  - **Description:** A dedicated module for uploading and checking identity verification status.
  - **Benefits:** Simulates real-world financial compliance.
  - **User impact:** Provides a realistic FinTech onboarding experience.
- **Feature Name:** Interactive Data Visualization
  - **Description:** Graphical charts powered by ApexCharts.
  - **Benefits:** Makes complex data easy to digest quickly.
  - **User impact:** Enhances the overall user experience through visual clarity.

---

## 12. Technology Stack
### Frontend Technologies
- **Vue 3 (Composition API):**
  - **Why used:** For building reactive, component-based user interfaces.
  - **Benefits:** Excellent performance, clean syntax (`<script setup>`), and great developer experience.
  - **Alternatives:** React, Angular.
  - **Role:** Handles all client-side rendering and user interactions.
- **Vite:**
  - **Why used:** As the frontend build tool.
  - **Benefits:** Lightning-fast Hot Module Replacement (HMR) and optimized production builds.
  - **Alternatives:** Webpack, Create-React-App.
  - **Role:** Compiles and serves the Vue application.
- **Tailwind CSS:**
  - **Why used:** For styling the application.
  - **Benefits:** Utility-first CSS allows rapid UI development without writing custom stylesheets.
  - **Alternatives:** Bootstrap, Vanilla CSS.
  - **Role:** Ensures the UI is responsive, modern, and visually consistent.
- **Pinia:**
  - **Why used:** For state management.
  - **Benefits:** Intuitive, type-safe alternative to Vuex, perfect for managing global authentication state.
  - **Alternatives:** Vuex, Redux (in React).
  - **Role:** Stores JWT tokens, user profiles, and global app state.

### Backend Technologies
- **Node.js:**
  - **Why used:** As the runtime environment for the server.
  - **Benefits:** Fast, asynchronous, event-driven architecture utilizing JavaScript across the entire stack.
  - **Alternatives:** Spring Boot (Java), Django (Python).
  - **Role:** Executes the backend server logic.
- **Express.js:**
  - **Why used:** As the web framework for Node.js.
  - **Benefits:** Minimalist, highly flexible, and excellent for building REST APIs quickly.
  - **Alternatives:** NestJS, Fastify.
  - **Role:** Handles API routing and HTTP requests/responses.

### Database
- **MongoDB:**
  - **Why used:** As the primary database.
  - **Benefits:** NoSQL document structure maps perfectly to JSON objects, allowing rapid development.
  - **Alternatives:** MySQL, PostgreSQL.
  - **Role:** Persistently stores users, wallets, and KYC data.
- **Mongoose:**
  - **Why used:** As an ODM (Object Data Modeling) library for MongoDB.
  - **Benefits:** Provides schema validation and relationship mapping.
  - **Role:** Bridges Node.js controllers and the MongoDB database.

### Authentication
- **JSON Web Tokens (JWT):**
  - **Why used:** For stateless authentication.
  - **Benefits:** No session data needs to be stored in the database; scales easily.
  - **Alternatives:** Session Cookies.
  - **Role:** Secures API routes by validating the token attached to requests.
- **Bcrypt:**
  - **Why used:** For password hashing.
  - **Benefits:** Adds salt to hashes, preventing rainbow-table attacks.
  - **Role:** Secures user passwords before storing them in MongoDB.

---

## 13. System Architecture
- **High-level architecture diagram:**
  `Client Browser (Vue) <---> REST API (Node/Express) <---> NoSQL DB (MongoDB)`
- **Frontend-backend communication flow:** The frontend utilizes Axios to send asynchronous HTTP requests (GET, POST) to backend REST endpoints. The backend processes the request and returns JSON responses.
- **Database architecture:** Document-based storage where the `User` document acts as the central entity. `Wallet` and `KYC` documents are linked to the `User` via an `ObjectId` reference.
- **Deployment architecture:** The Vue SPA is built into static files (`dist/`) and served via a CDN (e.g., Vercel/Netlify), while the Express API is hosted on a Node.js cloud provider (e.g., Render/AWS), connecting to a managed MongoDB Atlas cluster.
- **Component architecture:** Frontend is broken down into reusable `components` (e.g., `Navbar`, `Sidebar`, `ChartCard`) assembled within `views` (`Dashboard`, `Wallet`, `Auth`).

---

## 14. Folder Structure Explanation
```text
stocktrail-main/
├── backend/                  # Contains all Node.js/Express server code
│   ├── src/
│   │   ├── config/           # Database connection and environment variable configurations
│   │   ├── controllers/      # Core business logic for handling incoming API requests
│   │   ├── middlewares/      # Interceptors for JWT verification and error handling
│   │   ├── models/           # Mongoose schemas defining database structure
│   │   ├── routes/           # Express router files mapping URLs to Controllers
│   │   ├── services/         # Reusable logic abstracted away from controllers
│   │   └── utils/            # Helper functions (hashing, email generation, validation)
│   ├── server.js             # Main entry point that bootstraps the Express application
│   └── package.json          # Backend dependencies and scripts
└── frontend/                 # Contains all Vue 3 / Vite client code
    ├── src/
    │   ├── api/              # Axios instance configurations and API call wrappers
    │   ├── components/       # Reusable Vue UI components (Buttons, Inputs, Modals)
    │   ├── router/           # Vue Router definitions and navigation guards
    │   ├── stores/           # Pinia state management modules (AuthStore, UserStore)
    │   ├── views/            # Complete page layouts corresponding to routes
    │   └── main.js           # Vue application entry point, mounting plugins
    ├── index.html            # Root HTML template
    ├── vite.config.js        # Build tool configuration
    └── package.json          # Frontend dependencies and scripts
```
- **Module organization:** Logic is strictly separated. Routes only map URLs, Controllers handle HTTP logic, and Models handle DB interactions.
- **Code structure:** Follows the MVC (Model-View-Controller) design pattern on the backend and component-based architecture on the frontend.

---

## 19. Authentication & Authorization Flow
- **Login flow:** User enters credentials on the frontend -> Axios POSTs to `/api/auth/login` -> Backend finds user in DB -> Compares hashed password via bcrypt -> If valid, signs a JWT with the user's ID -> Returns JWT to frontend -> Frontend saves JWT in localStorage/Pinia and redirects to Dashboard.
- **Registration flow:** User enters details -> Axios POSTs to `/api/auth/register` -> Backend validates data -> Hashes password -> Creates new `User` document -> Generates initial `Wallet` -> Returns success message.
- **JWT token flow:** Stored on the client, the JWT is attached to the `Authorization: Bearer <token>` header by an Axios interceptor for every outgoing request to a protected API.
- **Password hashing:** Handled automatically by Mongoose pre-save hooks using bcrypt before a new user is inserted into the DB.
- **Role-based access:** (If implemented) The JWT payload contains the user's role. Middleware checks this role before allowing access to admin-specific routes.
- **Session handling:** Entirely stateless via JWT; no server-side session memory is required.
- **Protected APIs:** Any route in Express wrapped with the `authMiddleware` requires a valid JWT to proceed.

---

## 20. Complete Workflow Explanation
- **User request flow:** A user clicks "View Wallet".
- **Frontend workflow:** The Vue component dispatches a Pinia action to fetch the wallet. Axios interceptors attach the auth token.
- **Backend workflow:** Express receives the `GET /api/wallet` request. The `authMiddleware` intercepts it, verifies the JWT, and attaches `req.userId`. It then forwards the request to `WalletController.getWallet()`.
- **Database workflow:** The controller uses Mongoose to execute `Wallet.findOne({ userId: req.userId })`.
- **API lifecycle:** The data is retrieved from MongoDB, formatted by the controller, and sent back as a `200 OK` JSON response.
- **Data flow:** The JSON response reaches Axios, updates the Pinia state, and Vue's reactivity system automatically re-renders the DOM to display the new balance.
- **Error flow:** If the DB fails or the token is expired, the backend returns a `401` or `500` status code. Axios catches this error, and Vue triggers a toast notification to alert the user.

---

## 25. Performance Optimization
- **Optimization techniques used:** Code splitting on the frontend, indexing on the backend.
- **Lazy loading:** Vue Router utilizes dynamic imports (`component: () => import('./View.vue')`) so that JS bundles are only loaded when a user actually visits that page.
- **Efficient rendering:** Vue 3's Virtual DOM ensures only the changed elements (like a stock price or wallet balance) are re-rendered, not the entire page.
- **Query optimization:** MongoDB collections index the `email` field in `Users` and `userId` in `Wallets` to ensure rapid `O(1)` or `O(log N)` lookups.
- **API optimization:** Unnecessary data is stripped from Mongoose queries using projections (e.g., `select('-password')`).
- **Caching strategies:** The frontend uses Pinia to cache user data, minimizing redundant API calls if the user navigates between views.

---

## 26. Error Handling Strategy
- **Frontend error handling:** Axios interceptors globally catch API errors. `401 Unauthorized` errors trigger an automatic logout and redirect to the login page.
- **Backend error handling:** A centralized Express error-handling middleware catches all thrown errors and unhandled promise rejections, preventing the server from crashing.
- **API error responses:** All errors follow a strict, predictable JSON format: `{ success: false, error: "Human readable message" }`.
- **Validation handling:** 
  - *Frontend:* Vee-Validate and Yup provide immediate visual feedback if an email is malformed or a password is too short before the form is even submitted.
  - *Backend:* Express controllers validate `req.body` thoroughly before interacting with the database.
- **Logging strategy:** `console.error` and dedicated logging tools trace the stack error to simplify debugging in development.

---

## 27. UI/UX Documentation
- **Design principles:** Clean, minimalist, and data-centric. Uses ample whitespace and high contrast to ensure financial figures are highly readable.
- **Responsiveness:** Tailwind CSS's mobile-first utility classes (`flex-col md:flex-row`) ensure the dashboard looks perfect on mobile phones, tablets, and 4k desktop monitors.
- **User experience:** Fast, SPA navigation with no page reloads. Loading spinners provide feedback during API calls. Toast notifications confirm successful actions (like "KYC Uploaded").
- **Navigation structure:** A sticky sidebar for desktop users and a collapsible hamburger menu for mobile users to quickly jump between Dashboard, Wallet, and Profile.
- **Accessibility considerations:** Semantic HTML tags (`<nav>`, `<main>`), contrasting colors for text readability, and visual focus states on input fields to aid keyboard navigation.
