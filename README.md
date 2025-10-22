# TumdexClient

<div align="center">

![Tumdex Logo](assets//icons/TUMdex.png)

**Modern, Scalable E-Commerce Platform**

[![Angular](https://img.shields.io/badge/Angular-18.0-DD0031?style=flat&logo=angular&logoColor=white)](https://angular.io/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.4-3178C6?style=flat&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)
[![Material Design](https://img.shields.io/badge/Material_Design-18.0-757575?style=flat&logo=material-design&logoColor=white)](https://material.angular.io/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[Demo](#demo) • [Features](#features) • [Installation](#installation) • [Documentation](#documentation)

</div>

---

## 📖 About

**TumdexClient** is a cutting-edge e-commerce platform frontend built with Angular 18. It offers a comprehensive solution for modern online retail with an intuitive admin panel, dynamic product management, and seamless user experience. The platform is designed with scalability, performance, and user experience at its core.

### 🎯 Project Highlights

- **Modern Architecture**: Built with Angular 18 standalone components
- **Progressive Web App**: Full PWA support with offline capabilities
- **Real-time Updates**: SignalR integration for live notifications
- **SEO Optimized**: Dynamic routing with SEO-friendly URLs
- **Performance Focused**: Advanced monitoring and analytics
- **Secure & Scalable**: JWT authentication with role-based access control

---

![TumdexHomePage](docs/screenshots/tumdex.avif)

## ✨ Features

### 🛍️ E-Commerce Core

- **Product Management**
  - Advanced product catalog with multi-category support
  - Dynamic product features and specifications
  - Image gallery with drag-and-drop upload
  - Stock management and pricing controls
  - Brand association and filtering

- **Shopping Experience**
  - Intelligent search with real-time suggestions
  - Advanced filtering and sorting options
  - Shopping cart with persistent state
  - Wishlist/Favorites functionality
  - Order tracking and history

- **Category System**
  - Hierarchical category structure
  - SEO-friendly category pages
  - Custom category images and descriptions
  - Dynamic breadcrumb navigation

### 🎨 User Interface

- **Responsive Design**
  - Mobile-first approach
  - Bootstrap 5 integration
  - Material Design components
  - Custom SCSS styling

- **Dynamic Content**
  - Carousel/Slider management
  - Rich text editor for descriptions
  - Company logo customization
  - Newsletter subscription system

### 👥 User Management

- **Authentication**
  - Email/Password registration and login
  - Social login integration (Google, Facebook)
  - Password reset functionality
  - Email verification system

- **User Features**
  - Profile management
  - Order history
  - Saved addresses
  - Favorite products
  - Newsletter preferences

### 🔐 Admin Panel

- **Dashboard**
  - Real-time analytics
  - Sales statistics
  - Visitor tracking
  - Performance metrics

![Admin Dashboard](docs/screenshots/tumdexAdminDashboardPage.avif)

- **Content Management**
  - Product CRUD operations
  - Category management
  - Brand management
  - Feature/attribute system
  - Carousel management
  - Company logo updates

- **Order Management**
  - Order processing
  - Status updates
  - Customer information
  - Order details and tracking

- **User Administration**
  - User list and management
  - Role-based access control
  - Permission management
  - Authorization matrix

- **Performance Monitoring**
  - Real-time performance metrics
  - Resource usage tracking
  - Error monitoring
  - Analytics dashboard

![Performance Monitoring](docs/screenshots/tumdexAdminPerformancePage.avif)

### 🎯 Advanced Features

- **Progressive Web App (PWA)**
  - Offline mode support
  - Service worker integration
  - Install to home screen
  - Push notifications ready

- **Real-time Communication**
  - SignalR integration
  - Live notifications
  - Real-time updates
  - Admin alerts

- **SEO & Performance**
  - Dynamic meta tags
  - SEO-friendly URLs
  - Lazy loading
  - Code splitting
  - Optimized images

- **Analytics & Tracking**
  - Visitor tracking
  - User behavior analysis
  - Performance monitoring
  - Custom event tracking

---

## 🖼️ Screenshots

### Category Page
![Category Page](docs/screenshots/tumdexCategoryPAge.avif)

### Product Detail Page
![Product Detail](docs/screenshots/tumdexProductDetailPage.avif)

---

## 🛠️ Technology Stack

### Core
- **Angular 18.0** - Frontend framework with standalone components
- **TypeScript 5.4** - Type-safe development
- **RxJS 7.8** - Reactive programming

### UI/UX
- **Angular Material 18** - Material Design components
- **Bootstrap 5.3** - Responsive grid and utilities
- **Bootstrap Icons** - Icon set
- **Font Awesome 4.7** - Additional icons
- **Ngx-Spinner** - Loading animations
- **Ngx-Toastr** - Toast notifications
- **AlertifyJS** - Alert dialogs

### Features
- **@microsoft/signalr** - Real-time communication
- **@auth0/angular-jwt** - JWT token handling
- **@kolkov/angular-editor** - Rich text editor
- **ngx-file-drop** - File upload with drag & drop
- **chart.js** - Data visualization
- **ngx-mat-select-search** - Searchable select inputs

### Authentication
- **@abacritt/angularx-social-login** - Social authentication
- JWT authentication system
- Role-based access control

### PWA
- **@angular/service-worker** - Service worker management
- Offline functionality
- Cache management

---

## 📦 Installation

### Prerequisites

- Node.js (v18 or higher)
- npm or yarn
- Angular CLI (`npm install -g @angular/cli`)

### Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/muratfirtina/TumdexClient.git
   cd TumdexClient
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Configure environment**
   
   Update `src/environments/environment.ts` with your backend API URL:
   ```typescript
   export const environment = {
     production: false,
     baseUrl: 'https://your-api-url'
   };
   ```

4. **Run development server**
   ```bash
   npm start
   # or
   ng serve
   ```

5. **Navigate to** `http://localhost:4200/`

### Production Build

```bash
npm run build
# or
ng build --configuration production
```

Build artifacts will be stored in the `dist/tumdex-client/` directory.

---

## 📁 Project Structure

```
TumdexClient/
├── src/
│   ├── app/
│   │   ├── admin/              # Admin panel components
│   │   │   ├── components/     # Admin feature components
│   │   │   └── layout/         # Admin layout
│   │   ├── ui/                 # User interface components
│   │   │   ├── components/     # UI feature components
│   │   │   └── layout/         # UI layout
│   │   ├── base/              # Base components
│   │   ├── common/            # Shared components
│   │   ├── contracts/         # TypeScript interfaces
│   │   ├── dialogs/           # Dialog components
│   │   ├── directives/        # Custom directives
│   │   ├── guards/            # Route guards
│   │   ├── interceptors/      # HTTP interceptors
│   │   ├── pipes/             # Custom pipes
│   │   ├── services/          # Application services
│   │   │   ├── admin/         # Admin services
│   │   │   ├── common/        # Shared services
│   │   │   └── ui/            # UI services
│   │   └── constants/         # Application constants
│   ├── assets/                # Static assets
│   └── environments/          # Environment configurations
├── docs/                      # Documentation
│   └── screenshots/           # Application screenshots
└── public/                    # Public assets
```

---

## 🚀 Usage

### Development

```bash
# Start development server
npm start

# Run with specific configuration
ng serve --configuration development

# Run with SSL
ng serve --ssl
```

### Testing

```bash
# Run unit tests
npm test

# Run tests with coverage
ng test --code-coverage
```

### Building

```bash
# Development build
ng build --configuration development

# Production build
ng build --configuration production
```

---

## 🔧 Configuration

### Environment Variables

Configure your environment in `src/environments/`:

- `environment.ts` - Development configuration
- `environment.prod.ts` - Production configuration

```typescript
export const environment = {
  production: false,
  baseUrl: 'https://api.example.com'
};
```

### Angular Configuration

Customize Angular settings in `angular.json`:
- Build optimization
- Service worker settings
- Asset management
- Style preprocessing

---

## 🔐 Authentication & Authorization

The platform uses JWT-based authentication with role-based access control:

- **Public Routes**: Home, Products, Categories, etc.
- **Protected Routes**: Cart, Orders, Profile
- **Admin Routes**: Dashboard, Management panels

### User Roles

- **Admin**: Full system access
- **User**: Standard customer access
- **Guest**: Public content only

---

## 🎨 Styling

The project uses a combination of:
- **SCSS** for custom styling
- **Bootstrap 5** for responsive layout
- **Angular Material** for components
- **Custom theme** system

### Theme Customization

Modify `src/styles.scss` to customize the theme:
```scss
@use '@angular/material' as mat;

$custom-primary: mat.define-palette(mat.$indigo-palette);
$custom-accent: mat.define-palette(mat.$pink-palette);
```

---

## 📱 Progressive Web App (PWA)

The application includes full PWA support:

- ✅ Service Worker integration
- ✅ Offline functionality
- ✅ Install to home screen
- ✅ App manifest
- ✅ Caching strategies

Configure PWA settings in `ngsw-config.json`.

---

## 🔄 API Integration

The client communicates with a backend API. Key service categories:

### Admin Services
- Product Management
- Category Management
- Brand Management
- Order Management
- User Management
- Role Management

### UI Services
- Product Display
- Shopping Cart
- User Authentication
- Order Placement
- Search & Filter

### Common Services
- SignalR Hub
- File Upload
- Notifications
- Analytics

---

## 🌐 Internationalization (i18n)

The application is ready for internationalization:
- Translation files in `src/assets/i18n/`
- Language switching support
- RTL support ready

---

## 📊 Performance Monitoring

Built-in performance monitoring features:
- Real-time metrics
- Resource usage tracking
- Error logging
- User analytics
- Visitor tracking

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Coding Standards

- Follow Angular style guide
- Use TypeScript strict mode
- Write unit tests for new features
- Update documentation

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Murat Fırtına**

- GitHub: [@muratfirtina](https://github.com/muratfirtina)
- Project Link: [https://github.com/muratfirtina/TumdexClient](https://github.com/muratfirtina/TumdexClient)

---

## 🙏 Acknowledgments

- Angular Team for the amazing framework
- Material Design for the design system
- All contributors who helped improve this project

---

## 📞 Support

For support, please:
- Open an issue on GitHub
- Contact the development team
- Check the documentation

---

<div align="center">

**Made with ❤️ using Angular**

⭐ Star this repository if you find it helpful!

</div>
