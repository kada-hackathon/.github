# Nebwork - Kada Hackathon Organization

<div align="center">

**Modern Collaborative Work Management Platform**

[🌐 Live Application](https://nebwork.app) • [📖 Documentation](#documentation) • [🚀 Repositories](#repositories)

</div>

---

## 📋 Project Overview

### Goal
Nebwork is a comprehensive work management and collaboration platform designed to streamline team workflows, facilitate real-time communication, and enhance productivity. The platform consists of a modern React-based frontend and a robust Node.js backend API, providing an intuitive interface for work logging, chat functionality, document editing, and team collaboration.

### Main Features

#### 🎨 Frontend Features
- **🔐 Authentication & Authorization** - Secure login with protected routes and role-based access control
- **📝 Work Log Management** - Create, edit, and track work logs with version history
- **💬 Real-time Chat** - Integrated chatbot and messaging functionality
- **🤝 Collaboration Tools** - Team collaboration with friends list and collaborative document editing
- **📄 Rich Text Editor** - Powerful Tiptap-based editor with real-time collaboration features
- **📊 Document Management** - Preview and manage various document formats
- **🎨 Modern UI/UX** - Beautiful, responsive interface with dark/light theme support (shadcn/ui + Tailwind CSS)
- **📱 Mobile Responsive** - Fully responsive design for all device sizes
- **🔔 Notifications** - Toast notifications and real-time updates
- **👤 User Profiles** - Comprehensive user profile management
- **🛡️ Admin Dashboard** - Administrative interface for system management
- **📖 Blog System** - Create and publish blog posts with rich content

#### 🔧 Backend Features
- **🔒 JWT Authentication** - Secure session token management
- **📡 RESTful API** - Well-structured API endpoints under `/api/auth` and `/api/admin`
- **💾 MongoDB Integration** - Robust data persistence layer
- **📧 Email Services** - Automated email functionality for notifications
- **✅ Test Suite** - Comprehensive tests using Jest and Supertest
- **🔄 Auto-reload Support** - Development-friendly with nodemon support
- **🔐 Security** - Built-in security features and validation

#### 🏢 Organization Infrastructure
- **Organization Configuration** - Shared GitHub configurations and templates
- **CI/CD Workflows** - Reusable GitHub Actions workflows
- **Community Standards** - Standardized issue and pull request templates
- **Centralized Management** - Organization-level settings and dependency management

---

## 🗂 Repositories

### Frontend Repository
**Repository**: [kada-hackathon/front-end](https://github.com/kada-hackathon/front-end)

**Tech Stack**:
- React 18.3.1 with Vite 7.1.12
- shadcn/ui + Radix UI components
- Tailwind CSS for styling
- Tiptap collaborative editor
- TanStack React Query for state management
- React Hook Form + Zod validation

**Key Dependencies**: Yjs (collaborative editing), Recharts (data visualization), DOMPurify (security), React Router (navigation)

### Backend Repository
**Repository**: [kada-hackathon/backend](https://github.com/kada-hackathon/backend)

**Tech Stack**:
- Node.js with Express.js
- MongoDB database
- JWT for authentication
- Jest + Supertest for testing

**API Structure**: Exposes routes under `/api/auth` and `/api/admin`

### Organization Configuration
**Repository**: [kada-hackathon/.github](https://github.com/kada-hackathon/.github)

**Purpose**: Central configuration hub for the kada-hackathon organization containing shared workflows, templates, and organization-level settings.

---

## 🌐 Additional Information

### 🚀 Deployment & Live Access

#### Production Application
- **Live URL**: [https://nebwork.app](https://nebwork.app)
- **Platform**: Hosted on production infrastructure
- **Status**: Active and accessible

#### Staging Environment
- **DigitalOcean**: `frontend-he2bh.ondigitalocean.app`
- **Purpose**: Testing and preview builds

### 🔑 Test Accounts
For testing purposes, please contact the development team for test credentials. Ensure you use the password reset functionality if needed.

### 📖 Documentation

#### Frontend Documentation
- **API Configuration**: `src/config/api.js`
- **Component Structure**: See `src/components/` directory
- **Custom Hooks**: Available in `src/hooks/`
- **Utilities**: Check `src/lib/` and `src/utils/`

#### Backend Documentation
- **API Documentation**: `DOCS_API.md` (in backend repository)
- **Environment Variables**: See backend README for required `.env` fields
- **Test Suite**: Located in `src/test/` directory

#### Getting Started Guides

**Frontend Setup**:
```bash
# Clone and install
git clone https://github.com/kada-hackathon/front-end.git
cd front-end
npm install

# Start development server
npm run dev
# Access at http://localhost:8080
```

**Backend Setup**:
```bash
# Clone and install
git clone https://github.com/kada-hackathon/backend.git
cd backend
npm install

# Configure .env file (see DOCS_API.md)

# Start server
node index.js
# Or with auto-reload: npx nodemon index.js
```

### 🧪 Testing

**Frontend Tests**:
```bash
npm run test
```

**Backend Tests**:
```bash
npm test
```

Ensure MongoDB is running and environment variables are configured before running backend tests.

### 🤝 Contributing

We welcome contributions! Here's how to get started:

1. Fork the relevant repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes and commit (`git commit -m 'Add some AmazingFeature'`)
4. Push to your branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

**Code Style**:
- Follow ESLint rules configured in each project
- Use functional components with hooks (frontend)
- Write clean, self-documenting code
- Add tests for new features

### 📞 Contact & Support

- **Live Application**: [nebwork.app](https://nebwork.app)
- **Organization**: [github.com/kada-hackathon](https://github.com/kada-hackathon)
- **Issues**: Report issues in the respective repository

### 🏗 Architecture Overview

```
┌─────────────────┐
│   Frontend      │  React + Vite
│  (nebwork.app)  │  Port: 8080 (dev)
└────────┬────────┘
         │ HTTP/REST
         │
┌────────▼────────┐
│   Backend API   │  Node.js + Express
│ (/api/auth,     │  MongoDB
│  /api/admin)    │  JWT Auth
└─────────────────┘
```

### 📄 License

This project is part of the Kada Hackathon initiative. All rights reserved.

---

<div align="center">

**Made with ❤️ by the Nebwork Team**

*Last updated: November 2025*

</div>