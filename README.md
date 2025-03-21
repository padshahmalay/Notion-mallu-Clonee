# Notion-mallu-Clonee

A full-stack web application inspired by Notion that provides collaborative document editing, organization, and management. Built with React, Node.js, and PostgreSQL.

## [Notion Clone](https://notion-clonee.netlify.app/5ba1e6d7-72a2-4f76-a9a1-18b603dc7c35)

## 🚀 Features

- **Document Management**: Create, edit, organize, and delete documents
- **Rich Text Editor**: Support for various formatting options and media embedding
- **Real-time Collaboration**: Multiple users can edit documents simultaneously
- **User Authentication**: Secure login and registration system
- **Responsive Design**: Works seamlessly across desktop and mobile devices
- **Database Storage**: All content securely stored in PostgreSQL database

## 🛠️ Technology Stack

### Frontend
- **React**: UI library for building the user interface
- **Redux**: State management for predictable state container
- **Tailwind CSS**: Utility-first CSS framework for styling
- **Vite**: Next generation frontend tooling

### Backend
- **Node.js**: JavaScript runtime for the server
- **Express**: Web framework for Node.js
- **PostgreSQL**: Relational database for data storage
- **JWT**: Authentication using JSON Web Tokens

## 📂 Project Structure

```
notion-clone/
├── Notion-Clone-Backend-main/      # Backend codebase
│   ├── Config/                     # Configuration files
│   ├── Controllers/                # Route controllers
│   ├── Middlewares/                # Express middlewares
│   │   └── authentication.js       # Authentication middleware
│   ├── Models/                     # Database models
│   ├── Routes/                     # API routes
│   ├── .gitignore                 
│   ├── index.js                    # Entry point
│   ├── package-lock.json
│   └── package.json                # Dependencies
│
└── Notion-Clone-Frontend-main/     # Frontend codebase
    ├── public/                     # Static files
    ├── src/                        # Source code
    │   ├── assets/                 # Images, fonts, etc.
    │   ├── Auth/                   # Authentication components
    │   ├── Components/             # Reusable components
    │   ├── Pages/                  # Page components
    │   ├── Redux/                  # State management
    │   ├── App.css                 # Global styles
    │   ├── App.jsx                 # Main component
    │   ├── index.css               # Global styles
    │   └── main.jsx                # Entry point
    ├── .eslintrc.json              # ESLint configuration
    ├── .gitignore
    ├── index.html                  # HTML template
    ├── package-lock.json
    ├── package.json                # Dependencies
    └── vite.config.js              # Vite configuration
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- PostgreSQL (v12 or higher)

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/yourusername/notion-clone.git
   cd notion-clone
   ```

2. Set up the backend
   ```bash
   cd Notion-Clone-Backend-main
   npm install
   ```

3. Create a `.env` file in the backend directory with the following variables:
   ```
   PORT=5000
   DATABASE_URL=postgresql://username:password@localhost:5432/notionclone
   JWT_SECRET=your_jwt_secret
   ```

4. Set up the database
   ```bash
   # Create PostgreSQL database
   createdb notionclone
   
   # Run migrations (if applicable)
   npm run migrate
   ```

5. Set up the frontend
   ```bash
   cd ../Notion-Clone-Frontend-main
   npm install
   ```

6. Create a `.env` file in the frontend directory:
   ```
   VITE_API_URL=http://localhost:5000/api
   ```

### Running the Application

1. Start the backend server
   ```bash
   cd Notion-Clone-Backend-main
   npm run dev
   ```

2. Start the frontend development server
   ```bash
   cd Notion-Clone-Frontend-main
   npm run dev
   ```

3. Open your browser and navigate to `http://localhost:5173`

## 🧪 Testing

### Backend Tests
```bash
cd Notion-Clone-Backend-main
npm test
```

### Frontend Tests
```bash
cd Notion-Clone-Frontend-main
npm test
```

## 📝 API Documentation

The API documentation is available at `http://localhost:5000/api-docs` when the backend server is running.

### Main API Endpoints

- `POST /api/auth/register` - Register a new user
- `POST /api/auth/login` - Login a user
- `GET /api/documents` - Get all documents for a user
- `GET /api/documents/:id` - Get a specific document
- `POST /api/documents` - Create a new document
- `PUT /api/documents/:id` - Update a document
- `DELETE /api/documents/:id` - Delete a document

## 🤝 Contributing

1. Fork the repository
2. Create a new branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some amazing feature'`)
5. Push to the branch (`git push origin feature/amazing-feature`)
6. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

- [Notion](https://www.notion.so/) - For the inspiration
- [React](https://reactjs.org/) - UI Library
- [Node.js](https://nodejs.org/) - JavaScript runtime
- [PostgreSQL](https://www.postgresql.org/) - Database
- [Tailwind CSS](https://tailwindcss.com/) - CSS framework
- [Vite](https://vitejs.dev/) - Frontend build tool
