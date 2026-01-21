# NutriPlan 🥗

> A comprehensive Food, Nutrition & Fitness Planner web application built with vanilla JavaScript

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://david-samir-luis.github.io/NutriPlan/)
[![GitHub](https://img.shields.io/badge/github-repository-blue)](https://github.com/David-Samir-Luis/NutriPlan)
[![JavaScript](https://img.shields.io/badge/javascript-ES6+-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Demo](#demo)
- [Technologies](#technologies)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [API Reference](#api-reference)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## 🎯 Overview

NutriPlan is a modern web application designed to help users discover recipes, track nutrition, and maintain a healthy lifestyle. Built with vanilla JavaScript and powered by TheMealDB API, it provides an intuitive interface for meal planning and nutritional tracking.

### Key Highlights

- 🍳 **1000+ Recipes** from international cuisines
- 📊 **Real-time Nutrition Tracking** with visual progress indicators
- 🔍 **Smart Search** with category filtering
- 📱 **Responsive Design** optimized for all devices
- 🎨 **Modern UI/UX** with smooth animations and transitions

## ✨ Features

### 🍽️ Meals & Recipes

- **Dynamic Recipe Discovery**: Browse through a vast collection of recipes fetched from TheMealDB API
- **Category Filtering**: Filter by 12+ meal types (Beef, Chicken, Seafood, Vegan, Vegetarian, Dessert, etc.)
- **Smart Search**: Real-time search functionality to find recipes instantly
- **Cuisine Filtering**: Explore recipes from 15+ international cuisines
- **Recipe Details**: View comprehensive information including:
  - Ingredients list with measurements
  - Step-by-step cooking instructions
  - Video tutorials
  - Nutritional information
  - Cooking time and servings

### 🔍 Product Scanner

- **Product Search**: Search for packaged food products by name
- **Barcode Lookup**: Look up products using barcode numbers
- **Nutri-Score Filtering**: Filter products by nutrition quality ratings (A-E)
- **Category Browsing**: Browse by food categories (Cereals, Beverages, Snacks, etc.)
- **Nutrition Facts**: Access detailed nutritional information for each product

### 📈 Food Log & Tracking

- **Daily Nutrition Tracker**: Monitor daily intake of:
  - Calories (2000 kcal goal)
  - Protein (50g goal)
  - Carbohydrates (250g goal)
  - Fat (65g goal)
- **Visual Progress Bars**: Track your progress towards daily goals
- **Meal Logging**: One-click logging of meals from recipes
- **Weekly Overview**: View weekly nutrition trends with charts
- **Clear All Function**: Reset daily logs as needed

## 🎥 Demo

**Live Application**: [https://david-samir-luis.github.io/NutriPlan/](https://david-samir-luis.github.io/NutriPlan/)

### Screenshots

*Coming soon*

## 🛠️ Technologies

### Frontend
- **JavaScript ES6+**: Modules, async/await, template literals, destructuring
- **HTML5**: Semantic markup
- **CSS3**: Custom properties, flexbox, grid, animations

### APIs
- **TheMealDB API**: Recipe and meal data

### Tools & Deployment
- **Git**: Version control
- **GitHub Pages**: Hosting and deployment
- **ES6 Modules**: Code organization and modularity

## 📁 Project Structure

```
NutriPlan/
├── index.html              # Main HTML file
├── README.md               # Project documentation
└── src/
    ├── css/
    │   └── style.css       # Application styles
    └── js/
        ├── main.js         # Application entry point
        ├── api/
        │   └── mealdb.js   # API integration layer
        ├── state/
        │   └── appState.js # State management
        └── ui/
            └── components.js # UI components
```

### Architecture

The project follows a modular architecture with clear separation of concerns:

- **API Layer** (`api/mealdb.js`): Handles all external API calls
- **State Management** (`state/appState.js`): Centralized application state
- **UI Components** (`ui/components.js`): Reusable interface components
- **Main Controller** (`main.js`): Orchestrates the application flow

## 🚀 Installation

### Prerequisites

- Modern web browser (Chrome, Firefox, Safari, Edge)
- Text editor or IDE (VS Code recommended)
- Basic knowledge of HTML, CSS, and JavaScript

### Steps

1. **Clone the repository**
   ```bash
   git clone https://github.com/David-Samir-Luis/NutriPlan.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd NutriPlan
   ```

3. **Open in browser**
   - Simply open `index.html` in your web browser, or
   - Use a local development server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve
   ```

4. **Access the application**
   - Open your browser and navigate to `http://localhost:8000`

## 💡 Usage

### Browsing Recipes

1. Navigate to the **Meals & Recipes** page (default view)
2. Browse through recipe categories or use the search bar
3. Click on any category card to filter recipes
4. Click on a recipe card to view detailed information

### Searching for Meals

1. Use the search bar at the top of the Meals page
2. Type your desired meal name (e.g., "chicken", "pasta")
3. Results update dynamically as you type

### Logging Meals

1. Click on any recipe card to open the details modal
2. Click the **"Log This Meal"** button
3. View your logged meals in the **Food Log** page
4. Monitor your daily nutrition progress

### Product Scanning

1. Navigate to the **Product Scanner** page
2. Enter a product name or barcode number
3. Filter results using Nutri-Score ratings
4. Browse by food categories for quick access

### Tracking Nutrition

1. Go to the **Food Log** page
2. View your daily nutrition progress
3. Check the weekly overview chart
4. Use **"Clear All"** to reset your daily log

## 🔗 API Reference

### TheMealDB API

Base URL: `https://www.themealdb.com/api/json/v1/1/`

#### Endpoints Used

| Endpoint | Description | Usage |
|----------|-------------|-------|
| `/categories.php` | Get all meal categories | Fetch category list for filtering |
| `/search.php?s={query}` | Search meals by name | Implement search functionality |
| `/lookup.php?i={id}` | Get meal details by ID | Display recipe details |
| `/filter.php?c={category}` | Filter by category | Category-based filtering |
| `/filter.php?a={area}` | Filter by cuisine | Cuisine-based filtering |
| `/random.php` | Get random meal | Featured/random recipes |

#### Example Request

```javascript
// Fetch all categories
const response = await fetch('https://www.themealdb.com/api/json/v1/1/categories.php');
const data = await response.json();
console.log(data.categories);
```

## 🎨 Key Features Implementation

### Dynamic Content Loading
- Implemented skeleton loading states for optimal UX
- Smooth transitions between loading and loaded states
- Error handling for failed API requests

### State Management
- Centralized state management without frameworks
- Reactive updates to UI based on state changes
- Persistent state across page navigation

### Responsive Design
- Mobile-first approach
- Flexible grid layouts
- Responsive images and typography

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

### Contribution Guidelines

- Follow the existing code style
- Write clear commit messages
- Update documentation as needed
- Test your changes thoroughly

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Contact

**David Samir Luis**

- GitHub: [@David-Samir-Luis](https://github.com/David-Samir-Luis)
- Project Link: [https://github.com/David-Samir-Luis/NutriPlan](https://github.com/David-Samir-Luis/NutriPlan)

## 🙏 Acknowledgments

- **TheMealDB** for providing the free recipe API
- My instructor for guidance and mentorship throughout the project
- The web development community for inspiration and best practices

## 📊 Project Status

🟢 **Active Development** - Open to contributions and feedback

---

⭐ **If you find this project useful, please consider giving it a star!**

Made with ❤️ by David Samir Luis