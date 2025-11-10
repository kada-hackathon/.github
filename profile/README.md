
# Nebwork - Kada Hackathon Organization

<div align="center">

**Modern Collaborative Work Management Platform**

[🌐 Live Application](https://nebwork.app/) • [📖 Documentation](https://claude.ai/chat/9729fa39-00b1-4553-8bec-a31404f4a8f6#documentation) • [🚀 Repositories](https://claude.ai/chat/9729fa39-00b1-4553-8bec-a31404f4a8f6#repositories)

</div>

----------

## 📋 Project Overview

### The Problem

Lost institutional knowledge costs companies **$47 million annually** (per Fortune 500 company). When experienced employees leave, their valuable insights, processes, and expertise disappear with them, forcing companies to repeatedly train new hires from scratch.

### The Solution: Nebwork

Nebwork is a knowledge management platform that captures and preserves institutional knowledge before it walks out the door. We help companies retain critical insights from experienced professionals, especially those with 10+ years of experience, ensuring their expertise remains accessible even after they leave.

### How It Works

-   **📝 Work Log System** - Document daily work processes, insights, and solutions
-   **🏷️ Smart Tagging** - Organize content by topics, projects, or departments
-   **🔍 Fast Search** - Quickly find relevant documents and past experiences
-   **🤖 AI Chatbot** - Intelligent assistant to help find and retrieve information
-   **👥 Role-Based Access** - Secure sharing with appropriate permission levels

### Value Proposition

**For Companies**: Eliminate the need to train new employees from scratch by giving them direct access to insights from experienced professionals who have left the organization.

**For Employees**: Create a friendly, engaging platform where sharing knowledge feels natural and rewarding, not like extra work.

### MVP Features

Our Minimum Viable Product focuses on validating that employees are willing to share and retrieve knowledge through an engaging, lightweight platform:

-   ✅ **CRUD Blog System** - Create, read, update, and delete knowledge articles with rich media support
-   ✅ **Tagging & Organization** - Categorize content for easy discovery
-   ✅ **AI-Powered Chatbot** - Intelligent search and knowledge retrieval
-   ✅ **Advanced Search** - Find relevant information quickly
-   ✅ **Authentication & Roles** - Secure login with role-based permissions
-   ✅ **User-Friendly Interface** - Intuitive design that encourages knowledge sharing

### Main Features

#### 🎨 Frontend Features

-   **🔐 Authentication & Authorization** - Secure login with protected routes and role-based access control
-   **📝 Work Log Management** - Create, edit, and track work logs with version history
-   **💬 Real-time Chat** - Integrated chatbot and messaging functionality
-   **🤝 Collaboration Tools** - Team collaboration with friends list.
-   **📄 Rich Text Editor** - Powerful Tiptap-based editor with real-time collaboration features
-   **📊 Document Management** - Preview and manage various document formats
-   **🎨 Modern UI/UX** - Beautiful, responsive interface with dark/light theme support (shadcn/ui + Tailwind CSS)
-   **📱 Mobile Responsive** - Fully responsive design for all device sizes
-   **🔔 Notifications** - Toast notifications and real-time updates
-   **👤 User Profiles** - Comprehensive user profile management
-   **🛡️ Admin Dashboard** - Administrative interface for system management
-   **📖 Blog System** - Create and publish blog posts with rich content

#### 🔧 Backend Features

-   **🔒 JWT Authentication** - Secure session token management
-   **📡 RESTful API** - Well-structured API endpoints under `/api/auth` and `/api/admin`
-   **💾 MongoDB Integration** - Robust data persistence layer
-   **✅ Test Suite** - Comprehensive tests using Jest and Supertest
-   **🔄 Auto-reload Support** - Development-friendly with nodemon support
-   **🔐 Security** - Built-in security features and validation

#### 🏢 Organization Infrastructure

-   **Organization Configuration** - Shared GitHub configurations and templates
-   **CI/CD Workflows** - Reusable GitHub Actions workflows
-   **Community Standards** - Standardized issue and pull request templates
-   **Centralized Management** - Organization-level settings and dependency management

----------

## 🗂 Repositories

### Frontend Repository

**Repository**: [kada-hackathon/front-end](https://github.com/kada-hackathon/front-end)

**Tech Stack**:

-   React 18.3.1 with Vite 7.1.12
-   shadcn/ui + Radix UI components
-   Tailwind CSS for styling
-   Tiptap collaborative editor
-   TanStack React Query for state management
-   React Hook Form + Zod validation

**Key Dependencies**: Recharts (data visualization), DOMPurify (security), React Router (navigation)

### Backend Repository

**Repository**: [kada-hackathon/backend](https://github.com/kada-hackathon/backend)

**Tech Stack**:

-   Node.js with Express.js
-   MongoDB database
-   JWT for authentication
-   Jest + Supertest for testing

**API Structure**: Exposes routes under `/api/auth` and `/api/admin`

----------

## 🌐 Deployment & Infrastructure

### 🚀 Production Deployment

#### DigitalOcean App Platform

Both frontend and backend are deployed on **DigitalOcean App Platform**, providing:

-   **Automatic Deployments** - Connected to GitHub repositories for CI/CD
-   **Scalability** - Auto-scaling based on traffic and load
-   **SSL/TLS** - Automatic HTTPS certificate management
-   **Environment Management** - Secure environment variable handling
-   **Health Monitoring** - Built-in application health checks
-   **Zero-Downtime Deploys** - Rolling updates without service interruption

#### Live URLs

-   **Production Domain**: [https://nebwork.app](https://nebwork.app/)
-   **Staging Frontend**: `frontend-he2bh.ondigitalocean.app`
-   **Status**: Active and accessible

#### Deployment Architecture

```
┌──────────────────────────────────────┐
│   DigitalOcean App Platform          │
├──────────────────────────────────────┤
│                                      │
│  ┌─────────────────┐                │
│  │   Frontend App  │  React + Vite  │
│  │  (nebwork.app)  │  Port: 8080    │
│  └────────┬────────┘                │
│           │ HTTPS/REST              │
│           │                         │
│  ┌────────▼────────┐                │
│  │   Backend API   │  Node.js       │
│  │ (/api/auth,     │  Express       │
│  │  /api/admin)    │  JWT Auth      │
│  └────────┬────────┘                │
│           │                         │
│           ▼                         │
│  ┌─────────────────┐                │
│  │   MongoDB       │  Database      │
│  │   (Managed)     │                │
│  └─────────────────┘                │
│                                      │
└──────────────────────────────────────┘

```

### 🔑 Test Accounts

**Email**: sintaayu@yahoo.com  
**Password**: pass12345

----------

## 📖 Documentation

### Frontend Documentation

-   **API Configuration**: `src/config/api.js`
-   **Component Structure**: See `src/components/` directory
-   **Custom Hooks**: Available in `src/hooks/`
-   **Utilities**: Check `src/lib/` and `src/utils/`

### Backend Documentation

-   **API Documentation**: `DOCS_API.md` (in backend repository)
-   **Environment Variables**: See backend README for required `.env` fields
-   **Test Suite**: Located in `src/test/` directory

### Getting Started Guides

#### Frontend Setup

```bash
# Clone and install
git clone https://github.com/kada-hackathon/front-end.git
cd front-end
npm install

# Start development server
npm run dev
# Access at http://localhost:8080

```

#### Backend Setup

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

----------

## 🧪 Testing

### Frontend Tests

```bash
npm run test

```

### Backend Tests

```bash
npm test

```

Ensure MongoDB is running and environment variables are configured before running backend tests.

----------

## 🤝 Contributing

We welcome contributions! Here's how to get started:

1.  Fork the relevant repository
2.  Create a feature branch (`git checkout -b feature/AmazingFeature`)
3.  Make your changes and commit (`git commit -m 'Add some AmazingFeature'`)
4.  Push to your branch (`git push origin feature/AmazingFeature`)
5.  Open a Pull Request

### Code Style

-   Follow ESLint rules configured in each project
-   Use functional components with hooks (frontend)
-   Write clean, self-documenting code
-   Add tests for new features

----------

## 📞 Contact & Support

-   **Live Application**: [nebwork.app](https://nebwork.app/)
-   **Organization**: [github.com/kada-hackathon](https://github.com/kada-hackathon)
-   **Issues**: Report issues in the respective repository

----------

## 📄 License

This project is part of the Kada Hackathon initiative. All rights reserved.

----------

<div align="center">

**Made with ❤️ by the Nebwork Team**

_Last updated: November 2025_

</div>
