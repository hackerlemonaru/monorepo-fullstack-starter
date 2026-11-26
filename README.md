# 🚀 Monorepo Full-Stack Starter

A production-ready fullstack starter built with **Turborepo** monorepo architecture, featuring **Next.js 15** frontend, a high-performance **Rust (Axum)** backend, and a comprehensive **shadcn/ui** component library. Includes a **React** admin dashboard, **SQLx (PostgreSQL)**, **Docker** support, and complete developer tooling with **ESLint**, **Prettier**, **Husky**, and **Commitlint** for an optimal development experience.

<div align="center">

[![Docs](https://img.shields.io/badge/Documentation-Ready-blue?style=for-the-badge&logo=googledocs&logoColor=white)](https://docs-starter.dzikrisyairozi.com/docs)
[![Web Preview](https://img.shields.io/badge/Web_Preview-Live-orange?style=for-the-badge&logo=vercel&logoColor=white)](https://web-starter.dzikrisyairozi.com/)
[![Dashboard Preview](https://img.shields.io/badge/Dashboard-Live-purple?style=for-the-badge&logo=react&logoColor=white)](https://dashboard-starter.dzikrisyairozi.com/)

</div>

## ✨ Features

- 🏗️ **Turborepo** - High-performance build system for JavaScript/TypeScript monorepos
- ⚡ **Next.js 15** - React framework with App Router for Web & Docs
- 🦀 **Rust** - Ultra-fast backend API built with **Axum** and **SQLx**
- 🛠️ **TanStack Router** - Type-safe routing for the fast admin dashboard
- 🎨 **shadcn/ui** - Beautiful, accessible UI components built with Radix UI and Tailwind CSS
- ✨ **Framer Motion & Three.js** - Premium 3D animations and smooth transitions
- 🎯 **TypeScript** - Full type safety across all frontend applications
- 🎨 **Tailwind CSS** - Utility-first CSS framework
- 📱 **Responsive Design** - Mobile-first approach with dark/light mode support
- 🔧 **Developer Experience** - ESLint, Prettier, Husky, and Commitlint pre-configured
- 🌍 **Internationalization (i18n)** - Full multi-language support (English/Indonesian) across Web, Docs, and Dashboard
- 🐳 **Docker Ready** - Containerization support for easy deployment
- 🔄 **CI/CD** - GitHub Actions workflows included

## 📦 What's Inside?

This Monorepo includes the following packages and apps:

### Apps

- **`api`** - Rust backend API (Axum + SQLx)
- **`dashboard`** - Admin dashboard (TanStack Router + React)
- **`docs`** - Documentation site (Next.js + Fumadocs)
- **`web`** - Premium landing page (Next.js + React Three Fiber)

### Packages

- **`@repo/api-types`** - Auto-generated TS types from the Rust API
- **`@repo/i18n`** - Shared internationalization configuration and UI components
- **`@repo/ui`** - Shared React component library
- **`@repo/eslint-config`** - Shared ESLint configurations
- **`@repo/tailwind-config`** - Shared Tailwind CSS theme
- **`@repo/typescript-config`** - Shared TypeScript configurations

### Tools & Configuration

- **TypeScript** - Static type checking across all packages
- **ESLint** - Code linting with custom rules
- **Prettier** - Code formatting
- **Husky** - Git hooks for code quality
- **Commitlint** - Conventional commit message linting
- **Tailwind CSS** - Utility-first styling
- **Rust/Cargo** - Backend language and package manager
- **Docker** - Containerization support

## 🚀 Quick Start

### Prerequisites

- **Node.js** 22+
- **pnpm** (recommended package manager)
- **Git**

### Installation

1. **Use this template** (Recommended)
   Click the **"Use this template"** button at the top of the GitHub repository to create your own copy and start building immediately.

2. **Clone the repository**

   ```bash
   git clone https://github.com/dzikrisyairozi/monorepo-fullstack-starter.git
   cd monorepo-fullstack-starter
   ```

3. **Install dependencies**

   ```bash
   pnpm install
   ```

4. **Set up environment variables**

   ```bash
   # Copy environment files
   cp apps/api/.env.example apps/api/.env
   # Make sure to update your DATABASE_URL in apps/api/.env
   ```

5. **Set up the database** (if using the API)
   ```bash
   cd apps/api
   cargo sqlx database setup
   cd ../..
   ```

### Development

**Start all applications:**

```bash
pnpm dev
```

**Start specific applications:**

```bash
# Frontend only
pnpm dev:web

# Dashboard only
pnpm dev:dashboard

# Backend only
pnpm dev:api

# Documentation
pnpm dev:docs
```

**Access your applications:**

- 🌐 **Web App**: http://localhost:3000
- 🔧 **API**: http://localhost:3001
- 📚 **Docs**: http://localhost:3002
- 📊 **Dashboard**: http://localhost:5174

### Build

**Build all packages:**

```bash
pnpm build
```

**Build specific packages:**

```bash
pnpm build --filter=web
pnpm build --filter=dashboard
pnpm build --filter=api
pnpm build --filter=docs
```

## 🧩 Component Library

The `@repo/ui` package includes 40+ pre-built components from shadcn/ui:
