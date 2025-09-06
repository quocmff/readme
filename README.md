<!-- See: https://github.com/othneildrew/Best-README-Template -->
<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/quangquoc666/gjw-webapp">
    <img src="public/logo-with-text.webp" alt="Logo" width="320" height="80">
  </a>

<h3 align="center">Green Jade World - Backend API</h3>

  <p align="center">
    Laravel Backend API with Modern Development Workflow
    <br />
    <a href="#getting-started"><strong>Get Started »</strong></a>
    <br />
    <br />
    <a href="#built-with">Tech Stack</a>
    &middot;
    <a href="#usage">Development Workflow</a>
    &middot;
    <a href="#roadmap">Roadmap</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->

**Green Jade World Backend API** - Enterprise-ready Laravel application cho game với authentication system hoàn chỉnh, token management, audit logging và analytics dashboard.

**Key Features:**
- 🚀 **Authentication System**: Laravel Fortify + Sanctum với multi-provider OAuth (Local, Google, Facebook, Apple)
- 🔑 **Token Management**: Personal access tokens với ability checking & soft deletes
- 📊 **Audit Logging**: Enterprise audit system với change tracking & security monitoring
- 👑 **Admin Dashboard**: 6 analytics widgets với game statistics & system health monitoring
- 🔗 **RESTful API**: API versioning (/api/v1/) với device management & rate limiting
- 📚 **API Documentation**: Scramble auto-generated OpenAPI 3.0 spec với interactive docs
- 🗄️ **Database Schema**: Users, Accounts, Admins, Tokens, Audit Logs với soft deletes & UUID
- 🧪 **Testing Suite**: Comprehensive Pest tests với 95%+ coverage (6 loại tests)
- 🔒 **Security**: CSRF protection, rate limiting, input validation, account banning
- ⚡ **Performance**: Larastan L4, optimized indexes, eager loading ready
- 🤖 **AI-Powered**: Laravel Boost + Cursor Rules for intelligent development

<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With

**Core Technologies:**
* ![Laravel](https://img.shields.io/badge/Laravel-v12-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) - **Laravel v12** - The PHP Framework for Web Artisans
* ![Laravel Fortify](https://img.shields.io/badge/Laravel_Fortify-1.30-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) - **Laravel Fortify** - Frontend Authentication
* ![Laravel Sanctum](https://img.shields.io/badge/Laravel_Sanctum-4.0-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) - **Laravel Sanctum** - API Authentication
* ![PHP](https://img.shields.io/badge/PHP-8.4.5-777BB4?style=for-the-badge&logo=php&logoColor=white) - **PHP 8.4.5** - Server-side scripting language
* ![Pest](https://img.shields.io/badge/Pest-4.0-FF6B6B?style=for-the-badge&logo=pest&logoColor=white) - **Pest v4** - PHP Testing Framework

**Development Tools:**
* ![Filament](https://img.shields.io/badge/Filament-3.2-0055A4?style=for-the-badge&logo=laravel&logoColor=white) - **Filament** - Admin Panel
* ![Scramble](https://img.shields.io/badge/Scramble-0.12-0055A4?style=for-the-badge&logo=laravel&logoColor=white) - **Scramble** - API Documentation
* ![Larastan](https://img.shields.io/badge/Larastan-Level_4-0055A4?style=for-the-badge&logo=php&logoColor=white) - **Larastan Level 4** - Static Analysis
* ![Laravel Pint](https://img.shields.io/badge/Laravel_Pint-1.24-F05340?style=for-the-badge&logo=laravel&logoColor=white) - **Laravel Pint** - Code Formatter
* ![Laravel Boost](https://img.shields.io/badge/Laravel_Boost-1.1-FF2D20?style=for-the-badge&logo=laravel&logoColor=white) - **Laravel Boost** - AI Development

**Frontend & Database:**
* ![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-4.0-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white) - **Tailwind CSS v4** - Utility-first CSS
* ![Vite](https://img.shields.io/badge/Vite-6.0-646CFF?style=for-the-badge&logo=vite&logoColor=white) - **Vite** - Next generation frontend tooling
* ![MySQL](https://img.shields.io/badge/MySQL-5.7+-4479A1?style=for-the-badge&logo=mysql&logoColor=white) - **MySQL 5.7+** - Relational database

**Resources:** [Laravel Docs](https://laravel.com/docs/12.x) • [Laracasts](https://laracasts.com) • [Laravel Bootcamp](https://bootcamp.laravel.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

This guide will help you get the Green Jade World Backend API up and running on your local machine for development and testing purposes.

### Prerequisites

* **PHP 8.4.5+**
* **Composer 2.7+**
* **MySQL 5.7+**
* **Node.js 18+**
* **Laravel Boost** (recommended)

### Installation

```bash
# Clone & setup
git clone https://github.com/quangquoc666/gjw-webapp.git
cd gjw-webapp/backend

# Install dependencies
composer install
npm install

# Setup environment
cp .env.example .env
php artisan key:generate

# Configure database in .env
DB_CONNECTION=mysql
DB_DATABASE=green_jade_world
# ... other DB settings

# Setup database
php artisan migrate
composer run dev
```

### Development Workflow

```bash
# Quality checks
composer run quality  # All checks (lint + test)
composer run lint     # Static analysis + formatting
composer run test     # Test suite

# Development server
composer run dev      # Full dev environment (server + vite + queue)
```

### Code Quality Tools

- **Larastan Level 4** - Static analysis for PHP
- **Laravel Pint** - Code formatting
- **Pest v4** - Testing framework
- **Cursor Rules** - AI development guidelines

### AI-Powered Development

**Laravel Boost Tools:**
- `search-docs` - Real-time Laravel documentation với version-specific results
- `tinker` - PHP execution trong Laravel context với dependency injection
- `database-query` - Safe read-only database queries với SQL injection protection
- `browser-logs` - Frontend debugging và JavaScript error tracking
- `list-artisan-commands` - Dynamic command discovery và parameter validation
- `get-absolute-url` - URL generation với correct scheme/domain/port

**API Documentation:**
- `scramble:docs` - Generate OpenAPI 3.0 specification
- `/docs/api` - Interactive API documentation với Stoplight Elements
- Auto-updating docs cho tất cả API endpoints
- Multi-environment support (local, staging, production)

**Cursor Rules:** Auto-applies development guidelines, patterns và quality standards
- **Laravel v12** specific features và best practices
- **PHP 8.4** modern syntax và performance optimizations
- **Pest v4** testing patterns với browser testing capabilities
- **Security** guidelines với input validation và CSRF protection
- **Performance** optimizations với eager loading và query optimization

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ROADMAP -->
## Roadmap

### ✅ Completed
- [x] **Tech Stack**: PHP 8.4.5, Laravel v12, Pest v4, Tailwind v4 + Vite
- [x] **AI Integration**: Laravel Boost + Cursor Rules
- [x] **Code Quality**: Larastan L4, Laravel Pint, PSR-12
- [x] **Authentication System**: Laravel Fortify + Sanctum, multi-provider OAuth
- [x] **Token Management**: Personal access tokens với Filament admin interface
- [x] **Audit Logging**: Enterprise audit system với change tracking & security monitoring
- [x] **Admin Dashboard**: 6 analytics widgets với game statistics & system health monitoring
- [x] **Admin Panel**: Filament với user, account, token & audit logs management
- [x] **RESTful API**: API versioning, device management, rate limiting, CORS
- [x] **API Documentation**: Scramble OpenAPI 3.0 spec với interactive docs
- [x] **Database Schema**: Users, Accounts, Admins, Tokens, Audit Logs với soft deletes & UUID
- [x] **Testing Suite**: Comprehensive Pest tests với 95%+ coverage (6 loại tests)
- [x] **Security**: CSRF protection, rate limiting, input validation, account banning
- [x] **Development Workflow**: Optimized scripts & automation

### 🔄 In Progress
- [ ] **Game Economy**: Wallet system (Gems, Points, Transactions)
- [ ] **API Resources**: Eloquent API Resources cho response formatting
- [ ] **Frontend Integration**: React/Vue components cho admin panel

### 🚀 Planned
- [ ] **Performance**: Redis caching, CDN integration, query optimization
- [ ] **Testing**: Browser testing, API automation, load testing
- [ ] **Deployment**: Docker, CI/CD, monitoring, staging environment
- [ ] **Game Features**: Real-time notifications, leaderboards, achievements
- [ ] **Analytics**: User behavior tracking, performance metrics
- [ ] **Multi-tenancy**: Support multiple game worlds/regions

<p align="right">(<a href="#readme-top">back to top</a>)</p>





<!-- CONTACT -->
## Contact

**Quang Quoc** - Lead Developer
- Email: quangquoc666@gmail.com
- GitHub: [@quangquoc666](https://github.com/quangquoc666)
- Repository: [gjw-webapp](https://github.com/quangquoc666/gjw-webapp)

**🚀 Quick Setup:**
```bash
git clone https://github.com/quangquoc666/gjw-webapp.git
cd gjw-webapp/backend && composer install
npm install && cp .env.example .env
php artisan key:generate && php artisan migrate
composer run dev  # Start development
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

**Core Technologies:**
- **Laravel v12** - The PHP Framework for Web Artisans
- **Laravel Sanctum** - API Authentication & SPA support
- **PHP 8.4.5** - Modern server-side scripting với latest features

**AI & Development Tools:**
- **Laravel Boost** - AI-powered Laravel development với MCP server
- **Cursor IDE** - AI-first code editor với Laravel Rules
- **Larastan Level 4** - Static analysis với strict type checking
- **Pest v4** - Modern testing framework với browser testing
- **Filament** - Elegant admin panel cho Laravel

**Frontend & Build:**
- **Tailwind CSS v4** - Next-generation utility-first styling
- **Vite** - Lightning-fast build tool với HMR

**🙏 Special Thanks:**
- **Taylor Otwell** & Laravel Team
- **Nuno Maduro** - Laravel Boost & Pest
- **Dan Harrin** - Filament Admin Panel
- **Roman Zipp** - Laravel Scramble
- **Laravel Community** - Incredible ecosystem
- **Open Source Contributors**

**⭐ Star this repo if you find it helpful!**

<p align="right">(<a href="#readme-top">back to top</a>)</p>
