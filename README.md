# React-Recipe
<div align="center">

# 🍳 Tastebite - React Recipe

<p align="center">
  <img src="https://img.shields.io/badge/React-19.1.0-61DAFB?style=for-the-badge&logo=react&logoColor=white" alt="React" />
  <img src="https://img.shields.io/badge/Vite-7.0.4-646CFF?style=for-the-badge&logo=vite&logoColor=white" alt="Vite" />
  <img src="https://img.shields.io/badge/TailwindCSS-4.1.18-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white" alt="Tailwind" />
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="License" />
</p>

<p align="center">
  A modern, responsive recipe-sharing platform built with React and Tailwind CSS
</p>

[Report Bug](https://github.com/rohitrajak2004/React-Recipe/issues) · [Request Feature](https://github.com/rohitrajak2004/React-Recipe/issues)

</div>

---

## 📋 Table of Contents

- [About The Project](#about-the-project)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## 🎯 About The Project

**Tastebite** is a full-featured recipe management and sharing platform that allows users to discover, create, and share their favorite recipes. Built as a learning project to master React and modern frontend development, it showcases clean architecture, responsive design, and intuitive user experience.

### Why Tastebite?

- 🎨 **Beautiful UI**: Modern, clean interface with smooth animations
- 📱 **Fully Responsive**: Works seamlessly on desktop, tablet, and mobile
- 🔐 **User Authentication**: Secure login and signup functionality
- 👨‍💼 **Admin Dashboard**: Manage recipes and review user submissions
- 🎯 **Easy to Use**: Intuitive navigation and user-friendly forms

---

## ✨ Features

### Core Features

- **Recipe Discovery**: Browse through a curated collection of recipes across multiple categories (Dessert, Indian, Italian, etc.)
- **Detailed Recipe Pages**: View complete recipe information including ingredients, instructions, prep time, and servings
- **Recipe Submission**: Users can submit their own recipes for review
- **Category Filtering**: Filter recipes by cuisine type (Indian, Italian, Dessert, and more)
- **Search Functionality**: Find recipes quickly (coming soon!)
- **Star Ratings**: Visual rating system for recipes

### User Management

- **User Authentication**: Secure login and signup system
- **User Profiles**: Track submitted recipes and favorites
- **Admin Panel**: Dedicated dashboard for recipe moderation
- **Pending Recipe Queue**: Admin review system for user submissions

### UI/UX

- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Smooth Animations**: Enhanced with GSAP
- **Toast Notifications**: Real-time feedback with React Toastify
- **Beautiful Icons**: Lucide React icons throughout
- **Loading States**: Elegant loading indicators

---

## 🛠️ Tech Stack

### Frontend Framework
- **React 19.1.0** - UI library
- **React Router DOM 7.7.1** - Client-side routing
- **Vite 7.0.4** - Build tool and dev server

### Styling
- **Tailwind CSS 4.1.18** - Utility-first CSS framework
- **Custom CSS** - Additional styling

### Libraries & Tools
- **React Hook Form 7.71.1** - Form validation and management
- **React Toastify 11.0.5** - Toast notifications
- **Lucide React 0.562.0** - Icon library
- **GSAP 3.14.2** - Animation library
- **Axios 1.13.4** - HTTP client
- **Nanoid 5.1.6** - Unique ID generation

### Development Tools
- **ESLint 9.30.1** - Code linting
- **Vite Plugin React** - Fast refresh and JSX support

---

## 🚀 Getting Started

Follow these steps to get a local copy up and running.

### Prerequisites

Make sure you have the following installed:
- **Node.js** (v18 or higher)
- **npm** or **yarn** or **pnpm**

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/rohitrajak2004/React-Recipe.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd React-Recipe
   ```

3. **Install dependencies**
   ```bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   ```

4. **Start the development server**
   ```bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   ```

5. **Open your browser**
   ```text
   Navigate to http://localhost:5173
   ```

### Build for Production

```bash
npm run build
# or
yarn build
# or
pnpm build
```

The optimized files will be in the `dist` folder.

### Preview Production Build

```bash
npm run preview
# or
yarn preview
# or
pnpm preview
```

---

## 💡 Usage

### For Users

1. **Browse Recipes**: Explore the home page to discover featured recipes
2. **View Details**: Click on any recipe card to see full details
3. **Sign Up**: Create an account to submit your own recipes
4. **Submit Recipe**: Navigate to "Create Recipe" and fill out the form
5. **Track Submissions**: View your pending recipe submissions

### For Admins

1. **Login**: Use admin credentials to access the admin panel
2. **Review Submissions**: Check pending recipes in the admin dashboard
3. **Approve/Reject**: Manage user-submitted recipes
4. **Edit Recipes**: Update existing recipe information

### Authentication

⚠️ **For Local Development Only**

This application uses Context API for authentication state management. For local testing:

- The authentication system validates credentials against locally stored data
- No default credentials are provided in production
- For development/testing, you can create test accounts through the signup flow

**Security Notice**: Never commit real credentials to version control. Always use environment variables for sensitive data in production deployments.

---

## 📁 Project Structure

```text
React-Recipe/
├── public/              # Static assets
├── src/
│   ├── Auth/           # Authentication components
│   │   ├── Login.jsx
│   │   └── SignUp.jsx
│   ├── components/     # Reusable components
│   │   ├── Navbar.jsx
│   │   ├── Footer.jsx
│   │   ├── RecipeCard.jsx
│   │   ├── StarRating.jsx
│   │   ├── AdminNavbar.jsx
│   │   ├── AdminCard.jsx
│   │   ├── AdminPending.jsx
│   │   ├── AdminSingleRecipe.jsx
│   │   └── AdminUpdateRecipe.jsx
│   ├── context/        # Context API
│   │   └── RecipeData.jsx
│   ├── Pages/          # Page components
│   │   ├── Home.jsx
│   │   ├── Recipes.jsx
│   │   ├── SingleRecipe.jsx
│   │   ├── CreateRecipes.jsx
│   │   ├── About.jsx
│   │   └── Admin.jsx
│   ├── routes/         # Route configuration
│   │   └── Mainroutes.jsx
│   ├── utils/          # Utility modules
│   │   └── Axios.js
│   ├── style/          # CSS files
│   │   └── App.css
│   ├── App.jsx         # Main app component
│   └── main.jsx        # Entry point
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
└── eslint.config.js
```

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 👨‍💻 Contact

**Rohit Rajak** - [@rohit0git1](https://github.com/rohit0git1)

Project Link: [https://tastebite-seven.vercel.app/](https://tastebite-seven.vercel.app/)

---

## 🙏 Acknowledgments

- [React Documentation](https://react.dev)
- [Tailwind CSS](https://tailwindcss.com)
- [Lucide Icons](https://lucide.dev)
- [Vite](https://vitejs.dev)
- [React Router](https://reactrouter.com)
- [GSAP](https://greensock.com/gsap)

---

<div align="center">

### ⭐ Star this repo if you found it helpful!

Made with ❤️ by [Rohit Rajak](https://github.com/rohitrajak2004)

</div>
