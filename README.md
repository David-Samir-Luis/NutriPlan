# NutriPlan 🥗

> A Food, Nutrition & Fitness Planner web application for discovering recipes and tracking nutrition.

[![Live Demo](https://img.shields.io/badge/demo-live-brightgreen)](https://david-samir-luis.github.io/NutriPlan/)
[![JavaScript](https://img.shields.io/badge/javascript-ES6+-yellow)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## 📖 About

NutriPlan is a web application that helps users discover recipes, track nutrition, and maintain a healthy lifestyle. Built with vanilla JavaScript and powered by TheMealDB API, it provides access to thousands of recipes with detailed nutritional information, meal logging capabilities, and weekly nutrition tracking.

## ✨ Features

### 🍽️ Meals & Recipes
- Browse 1000+ recipes from international cuisines
- Filter by 12 meal categories (Beef, Chicken, Seafood, Vegan, Vegetarian, Desserts, etc.)
- Real-time search functionality
- Detailed recipe view with ingredients, instructions, and video tutorials
- One-click meal logging

### 🔍 Product Scanner
- Search packaged food products by name or barcode
- Filter by Nutri-Score ratings (A-E)
- Browse by food categories (Cereals, Beverages, Snacks, Dairy, etc.)
- View detailed nutrition facts

### 📊 Food Log & Tracking
- Track daily calories, protein, carbs, and fat
- Visual progress bars for nutrition goals
- Weekly nutrition analytics with charts
- Log meals directly from recipes
- View and manage all logged items

## 🛠️ Built With

- **JavaScript ES6+** - Modules, async/await, modern features
- **HTML5 & CSS3** - Semantic markup and modern styling
- **TheMealDB API** - Recipe and meal data
- **GitHub Pages** - Hosting and deployment

## 🚀 Getting Started

### Installation

1. Clone the repository
   ```bash
   git clone https://github.com/David-Samir-Luis/NutriPlan.git
   cd NutriPlan
   ```

2. Open `index.html` in your browser or use a local server
   ```bash
   python -m http.server 8000
   # or
   npx http-server
   ```

3. Navigate to `http://localhost:8000`

**No build process or dependencies required!**

## 📖 How To Use

### Browsing Recipes
1. Use the search bar to find recipes by name
2. Click category cards to filter by meal type
3. Select cuisine from dropdown to filter by region
4. Click any recipe card to view full details

### Logging Meals
1. Open a recipe detail modal
2. Click "Log This Meal" button
3. View logged meals in the Food Log page
4. Track your daily nutrition progress

### Product Scanner
1. Navigate to Product Scanner page
2. Search by product name or enter barcode number
3. Filter results by Nutri-Score rating
4. Browse by food categories

### Tracking Nutrition
1. Go to Food Log page
2. Monitor daily intake vs. goals (2000 kcal, 50g protein, 250g carbs, 65g fat)
3. View weekly nutrition trends
4. Use "Clear All" to reset daily log

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

**Architecture**: Modular design with separated API layer, state management, and UI components using ES6 modules.

## 🔗 API Reference

**TheMealDB API**: `https://www.themealdb.com/api/json/v1/1/`

| Endpoint | Purpose |
|----------|---------|
| `/categories.php` | Get all meal categories |
| `/search.php?s={query}` | Search recipes by name |
| `/lookup.php?i={id}` | Get recipe details |
| `/filter.php?c={category}` | Filter by category |
| `/filter.php?a={area}` | Filter by cuisine |

## 🎥 Demo

**Live App**: [https://david-samir-luis.github.io/NutriPlan/](https://david-samir-luis.github.io/NutriPlan/)

## 👨‍💻 Contact

**David Samir Luis**
- GitHub: [@David-Samir-Luis](https://github.com/David-Samir-Luis)
- Project: [NutriPlan Repository](https://github.com/David-Samir-Luis/NutriPlan)

## 🙏 Acknowledgments

- **TheMealDB** for the free recipe API

---

<div align="center">

⭐ **Star this repo if you find it useful!**

Made with ❤️ and JavaScript

</div>