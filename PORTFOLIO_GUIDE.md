# 🎯 Shravan's Hybrid Portfolio Projects

Welcome to my full-stack development portfolio! I've built two complementary projects showcasing my expertise in **Node.js, Vue.js, React, Docker, AWS, and Kubernetes**.

---

## 📋 Table of Contents

1. [Project 1: Developer Toolkit (Frontend)](#project-1-developer-toolkit-frontend)
2. [Project 2: Toolkit API Backend (Full-Stack)](#project-2-toolkit-api-backend-full-stack)
3. [Quick Start Guide](#quick-start-guide)
4. [Deployment Instructions](#deployment-instructions)
5. [Tech Stack Overview](#tech-stack-overview)

---

## 🎨 Project 1: Developer Toolkit (Frontend)

**Repository:** [developer-toolkit](https://github.com/shravannomula/developer-toolkit)  
**Live Demo:** [https://dev-toolkit.vercel.app](https://dev-toolkit.vercel.app)  
**Type:** Frontend | Vue 3 | TypeScript | PWA

### 📖 What is it?

A modern collection of 50+ developer tools built with Vue 3. It includes:
- JSON formatter & validator
- Base64 encoder/decoder
- UUID & ULID generator
- QR code generator
- Image converter & optimizer
- SQL formatter
- XML/YAML validator
- JWT decoder
- Regex tester
- Color converter
- And 40+ more tools!

### 🛠️ Tech Stack

```
Frontend:
├── Vue 3
├── TypeScript
├── Vite (build tool)
├── Pinia (state management)
├── Naive UI (component library)
├── UNO CSS (utility-first CSS)
└── PWA support

Testing:
├── Vitest (unit tests)
├── Playwright (E2E tests)
├── ESLint (linting)
└── Prettier (formatting)

Deployment:
├── Vercel (hosting)
├── Docker (containerization)
└── GitHub Actions (CI/CD)
```

### 📁 Project Structure

```
developer-toolkit/
├── src/
│   ├── tools/
│   │   ├── json-formatter/
│   │   ├── base64-encoder/
│   │   ├── uuid-generator/
│   │   └── ... (50+ tools)
│   ├── components/
│   │   ├── ToolCard.vue
│   │   ├── SearchBar.vue
│   │   └── ThemeToggle.vue
│   ├── stores/
│   │   └── tools.ts (Pinia)
│   ├── locales/
│   │   ├── en.json
│   │   ├── es.json
│   │   └── fr.json
│   ├── App.vue
│   └── main.ts
├── test/
│   ├── unit/
│   └── e2e/
├── Dockerfile
├── docker-compose.yml
├── vite.config.ts
└── package.json
```

### ✨ Key Features

- ✅ **50+ Developer Tools** - JSON, Base64, QR Code, UUID, JWT, SQL, XML, YAML, and more
- ✅ **Dark/Light Theme** - Beautiful UI with theme toggle
- ✅ **Multi-language Support** - English, Spanish, French (i18n)
- ✅ **Progressive Web App** - Works offline
- ✅ **Responsive Design** - Works on desktop, tablet, mobile
- ✅ **Type-Safe** - Full TypeScript support
- ✅ **Performance** - Optimized with Vite
- ✅ **Search** - Find tools instantly with fuzzy search
- ✅ **Copy to Clipboard** - One-click copy functionality
- ✅ **Tool Categories** - Organized by functionality

### 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/shravannomula/developer-toolkit.git
cd developer-toolkit

# Install dependencies
pnpm install

# Start development server
pnpm dev

# Build for production
pnpm build

# Run tests
pnpm test

# Run E2E tests
pnpm test:e2e

# Lint code
pnpm lint
```

### 🐳 Docker Deployment

```bash
# Build Docker image
docker build -t developer-toolkit:latest .

# Run container
docker run -d --name dev-toolkit -p 8080:80 developer-toolkit:latest

# Access at http://localhost:8080
```

### 🌐 Deploy to Vercel

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Set production environment
vercel --prod
```

---

## 🔌 Project 2: Toolkit API Backend (Full-Stack)

**Repository:** [toolkit-api-backend](https://github.com/shravannomula/toolkit-api-backend)  
**Live API:** [https://api-toolkit.herokuapp.com/docs](https://api-toolkit.herokuapp.com/docs)  
**Type:** Backend | Node.js | NestJS | TypeScript | Docker | Kubernetes

### 📖 What is it?

A production-ready REST API backend that powers developer tools with:
- User authentication (JWT, OAuth)
- Tool usage analytics
- File upload to AWS S3
- Email notifications
- Admin dashboard API
- Database support (PostgreSQL & MongoDB)
- API documentation (Swagger)
- Role-based access control

### 🛠️ Tech Stack

```
Backend:
├── Node.js
├── NestJS (framework)
├── TypeScript
├── Express.js (built-in)
└── Passport.js (auth)

Databases:
├── PostgreSQL (TypeORM)
├── MongoDB (Mongoose)
└── Redis (caching)

Authentication:
├── JWT
├── Google OAuth
├── Apple Sign-In
└── Facebook Login

File Storage:
├── AWS S3
└── Local storage

Email Service:
├── Nodemailer
└── SendGrid

DevOps:
├── Docker
├── Docker Compose
├── Kubernetes manifests
├── GitHub Actions
└── Helm charts

Testing:
├── Jest (unit tests)
├── Supertest (API tests)
├── E2E tests
└── Test coverage reporting

Documentation:
├── Swagger/OpenAPI
├── README documentation
└── API guides
```

### 📁 Project Structure

```
toolkit-api-backend/
├── src/
│   ├── auth/
│   │   ├── auth.controller.ts
│   │   ├── auth.service.ts
│   │   ├── jwt.strategy.ts
│   │   └── oauth.strategy.ts
│   ├── users/
│   │   ├── entities/
│   │   ├── dto/
│   │   ├── users.controller.ts
│   │   ├── users.service.ts
│   │   └── users.module.ts
│   ├── tools/
│   │   ├── entities/
│   │   ├── tools.controller.ts
│   │   ├── tools.service.ts
│   │   └── tools.module.ts
│   ├── analytics/
│   │   ├── analytics.controller.ts
│   │   └── analytics.service.ts
│   ├── file-upload/
│   │   ├── file.controller.ts
│   │   ├── file.service.ts
│   │   ├── s3.service.ts
│   │   └── file.module.ts
│   ├── mail/
│   │   ├── mail.service.ts
│   │   └── mail.module.ts
│   ├── database/
│   │   ├── migrations/
│   │   ├── seeds/
│   │   ├── data-source.ts
│   │   └── schemas/
│   ├── config/
│   │   ├── database.config.ts
│   │   ├── aws.config.ts
│   │   └── mail.config.ts
│   ├── app.module.ts
│   └── main.ts
├── test/
│   ├── auth.e2e-spec.ts
│   ├── users.e2e-spec.ts
│   ├── tools.e2e-spec.ts
│   └── jest-e2e.json
├── docker/
│   ├── Dockerfile
│   ├── Dockerfile.prod
│   └── .dockerignore
├── k8s/
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── configmap.yaml
│   ├── secret.yaml
│   └── ingress.yaml
├── docker-compose.yml
├── docker-compose.prod.yml
├── .github/workflows/
│   ├── ci.yml (tests)
│   ├── docker-build.yml
│   └── deploy.yml
└── package.json
```

### ✨ Key Features

- ✅ **User Authentication** - JWT + Social login (Google, Apple, Facebook)
- ✅ **CRUD Operations** - Full REST API for tools management
- ✅ **File Upload** - Integrated AWS S3 support
- ✅ **Email Service** - Nodemailer integration
- ✅ **Analytics** - Track tool usage and user behavior
- ✅ **Role-Based Access** - Admin, User, Guest roles
- ✅ **Database Support** - PostgreSQL (TypeORM) & MongoDB (Mongoose)
- ✅ **Database Migrations** - Auto-migration support
- ✅ **Seeding** - Pre-populate database with sample data
- ✅ **API Documentation** - Auto-generated Swagger docs
- ✅ **Error Handling** - Global exception filters
- ✅ **Validation** - Request validation with class-validator
- ✅ **Logging** - Structured logging system
- ✅ **Rate Limiting** - Prevent API abuse
- ✅ **Docker Support** - Multi-stage builds for production
- ✅ **Kubernetes Ready** - YAML configs for K8s deployment
- ✅ **CI/CD Pipeline** - GitHub Actions for automated testing & deployment
- ✅ **E2E Tests** - Complete API test coverage

### 📊 API Endpoints

```
Authentication:
POST   /api/auth/signup              - Register new user
POST   /api/auth/signin              - Login user
POST   /api/auth/refresh-token       - Refresh JWT token
GET    /api/auth/oauth/google        - Google OAuth login
GET    /api/auth/oauth/apple         - Apple Sign-In

Users:
GET    /api/users                    - List all users (admin)
GET    /api/users/:id                - Get user by ID
PATCH  /api/users/:id                - Update user profile
DELETE /api/users/:id                - Delete user (admin)

Tools:
GET    /api/tools                    - List all tools
GET    /api/tools/:id                - Get tool details
POST   /api/tools                    - Create new tool (admin)
PATCH  /api/tools/:id                - Update tool (admin)
DELETE /api/tools/:id                - Delete tool (admin)

File Upload:
POST   /api/files/upload             - Upload file to S3
GET    /api/files/:fileId            - Download file

Analytics:
GET    /api/analytics/usage          - Get tool usage stats
GET    /api/analytics/users          - Get user statistics
POST   /api/analytics/track          - Track tool usage

Admin:
GET    /api/admin/dashboard          - Admin dashboard data
GET    /api/admin/users              - User management
GET    /api/admin/reports            - System reports
```

### 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/shravannomula/toolkit-api-backend.git
cd toolkit-api-backend

# Install dependencies
npm install

# Copy environment file
cp .env.example .env

# Update .env with your configuration
# - Database credentials
# - AWS S3 credentials
# - JWT secret
# - OAuth credentials
# - Email service credentials

# Run database migrations
npm run migration:run

# Seed database (optional)
npm run seed:run

# Start development server
npm run start:dev

# Build for production
npm run build

# Run production server
npm run start:prod

# Run tests
npm test

# Run E2E tests
npm run test:e2e

# Run with coverage
npm run test:cov

# Generate API documentation (auto-generated)
# Access at http://localhost:3000/api/docs
```

### 🐳 Docker Deployment

```bash
# Build development image
docker build -f docker/Dockerfile -t toolkit-api:dev .

# Build production image
docker build -f docker/Dockerfile.prod -t toolkit-api:prod .

# Run with Docker Compose
docker-compose up -d

# Run production environment
docker-compose -f docker-compose.prod.yml up -d

# Access API at http://localhost:3000
# Swagger docs at http://localhost:3000/api/docs
```

### ☸️ Kubernetes Deployment

```bash
# Create namespace
kubectl create namespace toolkit

# Apply configurations
kubectl apply -f k8s/configmap.yaml -n toolkit
kubectl apply -f k8s/secret.yaml -n toolkit
kubectl apply -f k8s/deployment.yaml -n toolkit
kubectl apply -f k8s/service.yaml -n toolkit
kubectl apply -f k8s/ingress.yaml -n toolkit

# Check deployment
kubectl get deployments -n toolkit
kubectl get pods -n toolkit
kubectl get services -n toolkit

# View logs
kubectl logs -f deployment/toolkit-api -n toolkit

# Scale deployment
kubectl scale deployment toolkit-api --replicas=3 -n toolkit

# Update deployment
kubectl set image deployment/toolkit-api \
  toolkit-api=toolkit-api:v1.1.0 -n toolkit
```

### 📦 Environment Variables (.env)

```env
# Server
NODE_ENV=production
PORT=3000
API_URL=https://api-toolkit.herokuapp.com

# Database - PostgreSQL
DATABASE_TYPE=postgres
DATABASE_HOST=localhost
DATABASE_PORT=5432
DATABASE_USER=postgres
DATABASE_PASSWORD=your_password
DATABASE_NAME=toolkit_db

# Database - MongoDB (optional)
MONGO_URI=mongodb://localhost:27017/toolkit

# JWT
JWT_SECRET=your_jwt_secret_key_here
JWT_EXPIRATION=24h

# AWS S3
AWS_ACCESS_KEY_ID=your_aws_key
AWS_SECRET_ACCESS_KEY=your_aws_secret
AWS_S3_BUCKET=your_bucket_name
AWS_S3_REGION=us-east-1

# OAuth - Google
GOOGLE_CLIENT_ID=your_google_client_id
GOOGLE_CLIENT_SECRET=your_google_secret

# OAuth - Apple
APPLE_CLIENT_ID=your_apple_client_id
APPLE_TEAM_ID=your_apple_team_id

# OAuth - Facebook
FACEBOOK_APP_ID=your_facebook_app_id
FACEBOOK_APP_SECRET=your_facebook_secret

# Email Service
MAIL_HOST=smtp.gmail.com
MAIL_PORT=587
MAIL_USER=your_email@gmail.com
MAIL_PASSWORD=your_app_password
MAIL_FROM=noreply@toolkit.dev

# Logging
LOG_LEVEL=debug
LOG_FORMAT=json
```

---

## 🚀 Quick Start Guide

### Prerequisites

```bash
# Required
- Node.js >= 16.x
- npm >= 8.x or pnpm >= 9.x
- Docker & Docker Compose
- Git

# Optional
- PostgreSQL 14+
- MongoDB 6+
- Redis 7+
- AWS account (for S3)
- Vercel account (for frontend deployment)
```

### Installation Steps

#### 1️⃣ Frontend Setup (Developer Toolkit)

```bash
# Clone frontend
git clone https://github.com/shravannomula/developer-toolkit.git
cd developer-toolkit

# Install & run
pnpm install
pnpm dev

# Access at http://localhost:5173
```

#### 2️⃣ Backend Setup (Toolkit API)

```bash
# Clone backend
git clone https://github.com/shravannomula/toolkit-api-backend.git
cd toolkit-api-backend

# Install dependencies
npm install

# Setup environment
cp .env.example .env

# Setup databases
docker-compose up -d

# Run migrations
npm run migration:run

# Seed database
npm run seed:run

# Start server
npm run start:dev

# Access at http://localhost:3000
# Swagger docs at http://localhost:3000/api/docs
```

#### 3️⃣ Connect Frontend & Backend

Update frontend API URL in `src/config/api.ts`:

```typescript
export const API_BASE_URL = 'http://localhost:3000/api';
```

---

## 🌐 Deployment Instructions

### Frontend Deployment (Vercel)

```bash
cd developer-toolkit

# Install Vercel CLI
npm i -g vercel

# Deploy
vercel

# Set production
vercel --prod

# Get live URL
# Your app is live at: https://developer-toolkit.vercel.app
```

### Backend Deployment (Heroku)

```bash
cd toolkit-api-backend

# Login to Heroku
heroku login

# Create app
heroku create your-toolkit-api

# Set environment variables
heroku config:set NODE_ENV=production
heroku config:set JWT_SECRET=your_secret
heroku config:set DATABASE_URL=your_postgres_url
heroku config:set AWS_ACCESS_KEY_ID=your_key
heroku config:set AWS_SECRET_ACCESS_KEY=your_secret

# Deploy
git push heroku main

# View logs
heroku logs --tail

# Open app
heroku open
```

### Backend Deployment (Docker + AWS EC2)

```bash
# Build image
docker build -f docker/Dockerfile.prod -t toolkit-api:latest .

# Tag for ECR
docker tag toolkit-api:latest \
  123456789.dkr.ecr.us-east-1.amazonaws.com/toolkit-api:latest

# Push to ECR
docker push 123456789.dkr.ecr.us-east-1.amazonaws.com/toolkit-api:latest

# Deploy to EC2
docker pull 123456789.dkr.ecr.us-east-1.amazonaws.com/toolkit-api:latest
docker run -d -p 80:3000 \
  --env-file .env.prod \
  123456789.dkr.ecr.us-east-1.amazonaws.com/toolkit-api:latest
```

### Backend Deployment (Kubernetes)

```bash
# Create cluster
kubectl create cluster toolkit

# Create namespace
kubectl create namespace toolkit

# Deploy
kubectl apply -f k8s/ -n toolkit

# Verify
kubectl get all -n toolkit

# Scale
kubectl scale deployment toolkit-api --replicas=3 -n toolkit
```

---

## 🛠️ Tech Stack Overview

### Frontend Technology Matrix

| Technology | Purpose | Why Chosen |
|-----------|---------|-----------|
| Vue 3 | Frontend framework | Lightweight, reactive, excellent DX |
| TypeScript | Type safety | Catch errors early, better IDE support |
| Vite | Build tool | Fast, modern, ESM support |
| Pinia | State management | Simple, Vue 3 native |
| Naive UI | Component library | Beautiful, accessible, customizable |
| UNO CSS | Styling | Atomic CSS, smaller bundle size |
| Vitest | Unit testing | Fast, Vue 3 native |
| Playwright | E2E testing | Reliable, cross-browser support |

### Backend Technology Matrix

| Technology | Purpose | Why Chosen |
|-----------|---------|-----------|
| Node.js | Runtime | JavaScript backend, async/await |
| NestJS | Framework | Scalable, modular, DI support |
| TypeScript | Type safety | Enterprise-grade type checking |
| Express | HTTP server | Fast, lightweight, industry standard |
| PostgreSQL | Primary DB | Reliable, ACID compliant, JSON support |
| MongoDB | Secondary DB | Flexible schema, fast aggregation |
| Redis | Caching | Fast in-memory cache, session store |
| JWT | Authentication | Stateless, secure token auth |
| Passport.js | Auth strategies | Multiple OAuth provider support |
| AWS S3 | File storage | Scalable, cost-effective storage |
| Nodemailer | Email | Easy SMTP integration |
| Jest | Testing | Fast, comprehensive test framework |
| Docker | Containerization | Consistent environment, easy scaling |
| Kubernetes | Orchestration | Auto-scaling, load balancing, resilience |

---

## 📊 Development Workflow

### Git Strategy

```bash
# Main development branch
main (production-ready)

# Feature branches
feature/add-new-tool
feature/authentication
feature/analytics

# Bugfix branches
bugfix/fix-jwt-validation

# Release branches
release/v1.1.0

# Hotfix branches
hotfix/critical-security-patch
```

### CI/CD Pipeline

```
GitHub Push
    ↓
GitHub Actions Triggered
    ├── Run Tests (Jest, Vitest)
    ├── Run Linter (ESLint)
    ├── Build Code (Vite, NestJS)
    ├── Build Docker Images
    └── Upload to Registry
        ↓
    Deploy to Staging
        ├── Run E2E Tests
        ├── Performance Tests
        └── Security Scan
            ↓
        Deploy to Production
            ├── Gradual Rollout (10% → 50% → 100%)
            ├── Health Checks
            └── Monitoring & Alerts
```

---

## 📚 Learning Resources

### Frontend
- [Vue 3 Official Docs](https://vuejs.org/)
- [NaiveUI Documentation](https://www.naiveui.com/)
- [Vite Guide](https://vitejs.dev/)
- [Pinia Documentation](https://pinia.vuejs.org/)

### Backend
- [NestJS Documentation](https://docs.nestjs.com/)
- [TypeORM Guide](https://typeorm.io/)
- [Passport.js Strategies](http://www.passportjs.org/)
- [Docker Best Practices](https://docs.docker.com/develop/dev-best-practices/)

### DevOps
- [Kubernetes Official](https://kubernetes.io/docs/)
- [Docker Compose](https://docs.docker.com/compose/)
- [GitHub Actions](https://docs.github.com/en/actions)
- [AWS S3 Guide](https://docs.aws.amazon.com/s3/)

---

## 🤝 Contributing

Both projects welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

---

## 📝 License

- **Developer Toolkit**: GNU General Public License v3.0
- **Toolkit API Backend**: MIT License

---

## 📞 Contact & Support

- **GitHub**: [@shravannomula](https://github.com/shravannomula)
- **LinkedIn**: [Shravan Kumar Nomula](https://www.linkedin.com/in/shravannomula)
- **YouTube**: [@shravannomula](https://www.youtube.com/@shravannomula)
- **Medium**: [@shravannomula](https://medium.com/@shravannomula)

---

## 🎓 What You'll Learn

### Frontend Skills
✅ Modern Vue 3 composition API  
✅ TypeScript advanced patterns  
✅ Component-driven architecture  
✅ State management with Pinia  
✅ E2E testing strategies  
✅ PWA development  
✅ Responsive design  
✅ Performance optimization  

### Backend Skills
✅ NestJS modular architecture  
✅ RESTful API design  
✅ Database design & migrations  
✅ Authentication & authorization  
✅ File upload handling  
✅ Email service integration  
✅ Error handling & logging  
✅ Testing best practices  

### DevOps Skills
✅ Docker containerization  
✅ Docker Compose for local development  
✅ Kubernetes deployment  
✅ CI/CD with GitHub Actions  
✅ AWS S3 integration  
✅ Environment management  
✅ Monitoring & logging  
✅ Performance optimization  

---

**Happy Coding! 🚀**
