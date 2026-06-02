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

### ✨ Key Features

- ✅ **50+ Developer Tools**
- ✅ **Dark/Light Theme**
- ✅ **Multi-language Support** (i18n)
- ✅ **Progressive Web App**
- ✅ **Responsive Design**
- ✅ **Type-Safe** TypeScript
- ✅ **Performance Optimized**
- ✅ **Fuzzy Search**

### 🚀 Quick Start

```bash
git clone https://github.com/shravannomula/developer-toolkit.git
cd developer-toolkit
pnpm install
pnpm dev
```

---

## 🔌 Project 2: Toolkit API Backend (Full-Stack)

**Repository:** [toolkit-api-backend](https://github.com/shravannomula/toolkit-api-backend)  
**Live API:** [https://api-toolkit.herokuapp.com/docs](https://api-toolkit.herokuapp.com/docs)  
**Type:** Backend | Node.js | NestJS | TypeScript | Docker | Kubernetes

### 📖 What is it?

A production-ready REST API backend that powers developer tools with authentication, analytics, file upload, and more.

### ✨ Key Features

- ✅ **User Authentication** (JWT + OAuth)
- ✅ **CRUD Operations**
- ✅ **AWS S3 File Upload**
- ✅ **Email Service**
- ✅ **Analytics & Tracking**
- ✅ **Role-Based Access**
- ✅ **PostgreSQL & MongoDB Support**
- ✅ **Swagger Documentation**
- ✅ **Docker & Kubernetes Ready**
- ✅ **GitHub Actions CI/CD**

### 🚀 Quick Start

```bash
git clone https://github.com/shravannomula/toolkit-api-backend.git
cd toolkit-api-backend
npm install
cp .env.example .env
docker-compose up -d
npm run migration:run
npm run start:dev
```

---

## 💻 Tech Stack

### Frontend
- Vue 3, TypeScript, Vite, Pinia, Naive UI, UNO CSS
- Testing: Vitest, Playwright
- Deployment: Vercel, Docker

### Backend
- Node.js, NestJS, TypeScript, Express.js
- Databases: PostgreSQL (TypeORM), MongoDB (Mongoose)
- Auth: JWT, Passport.js (OAuth)
- Cloud: AWS S3, Email Service
- Testing: Jest, Supertest
- DevOps: Docker, Kubernetes, GitHub Actions

---

## 🌐 Deployment

### Frontend (Vercel)
```bash
cd developer-toolkit
npm i -g vercel
vercel --prod
```

### Backend (Heroku)
```bash
cd toolkit-api-backend
heroku login
heroku create your-api
git push heroku main
```

### Backend (Docker + AWS)
```bash
docker build -f docker/Dockerfile.prod -t toolkit-api:latest .
docker tag toolkit-api:latest YOUR_ECR_REPO:latest
docker push YOUR_ECR_REPO:latest
```

### Backend (Kubernetes)
```bash
kubectl create namespace toolkit
kubectl apply -f k8s/ -n toolkit
```

---

## 📚 Learning Resources

- [Vue 3 Docs](https://vuejs.org/)
- [NestJS Docs](https://docs.nestjs.com/)
- [TypeORM Guide](https://typeorm.io/)
- [Docker Best Practices](https://docs.docker.com/develop/dev-best-practices/)
- [Kubernetes Official](https://kubernetes.io/docs/)

---

## 🎓 Skills Showcase

### Frontend Skills
✅ Vue 3 Composition API  
✅ TypeScript patterns  
✅ Component architecture  
✅ State management  
✅ E2E testing  
✅ PWA development  

### Backend Skills
✅ NestJS architecture  
✅ RESTful API design  
✅ Database design  
✅ Authentication  
✅ File uploads  
✅ Email service  

### DevOps Skills
✅ Docker containerization  
✅ Kubernetes deployment  
✅ CI/CD pipelines  
✅ AWS integration  
✅ Environment management  

---

**Happy Coding! 🚀**
