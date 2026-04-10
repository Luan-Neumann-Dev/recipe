# Recipe App
 
> Browse and search thousands of recipes with detailed ingredients, nutritional facts, and preparation info — powered by the Edamam Recipe API.

[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org/)
[![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-2-764ABC?style=for-the-badge&logo=redux&logoColor=white)](https://redux-toolkit.js.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-3-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)](https://tailwindcss.com/)
[![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=for-the-badge&logo=vite&logoColor=white)](https://vitejs.dev/)

![Project Preview](https://github.com/user-attachments/assets/a93ac5ce-82ee-4d87-b78b-2541c69b9cbe)
![Project Preview](https://github.com/user-attachments/assets/092d2020-6f98-46c7-8809-cbe60ced91d0)
![Project Preview](https://github.com/user-attachments/assets/7466bcf7-383a-4252-8c0c-4b05f47c23eb)
![Project Preview](https://github.com/user-attachments/assets/d7033916-e4cc-492f-8d10-5d7163a27187)

<h4 align='center'>
  <a href='recipe-app-swart-ten.vercel.app'>Click here to view the project</a>
</h4>

## 🎯 About
 
Recipe App is a React SPA that lets users explore recipes by category or cuisine type, search by keyword, and view detailed recipe pages with ingredients, nutritional breakdown, preparation time, and calorie count — all fetched in real time from the Edamam Recipe API.
 
## ✨ Features

- 🔍 **Recipe Search** - Search recipes by any keyword with paginated results
- 🍽️ **Category & Cuisine Browsing** - Filter by meal type or cuisine (Italian, Asian, Mexican, etc.)
- 📖 **Detailed Recipe Page** - Full breakdown of ingredients, nutrients, health labels, prep time and calories
- 🖼️ **Image Lightbox** - View recipe images in multiple sizes with lightbox2
- ⏳ **Async State Management** - Loading, success and error states handled via Redux Toolkit
- 📱 **Responsive Layout** - Mobile-friendly design built with Tailwind CSS
- 🔄 **Pagination** - "Next Page" support using the API's cursor-based pagination
 
## 🛠️ Built With

- **React 18** — Component architecture and hooks
- **Redux Toolkit** — Global state with `createSlice`, `createEntityAdapter` and `createAsyncThunk`
- **Tailwind CSS** — Utility-first styling
- **Axios** — HTTP client for API requests
- **React Router DOM v6** — Multi-page routing with `createBrowserRouter`
- **React Slick** — Carousel components for banner and category sliders
- **Lightbox2** — Image gallery viewer on the single recipe page
- **Edamam Recipe API** — Source of all recipe data

## 🚀 Getting Started
 
### Prerequisites
 
- Node.js >= 18
- Edamam API credentials — [get them here](https://developer.edamam.com/)

### Installation
 
```bash
# Clone the repository
git clone https://github.com/Luan-Neumann-Dev/recipe.git
 
# Navigate to project directory
cd recipe
 
# Install dependencies
npm install
```

### API Setup
 
Add your Edamam credentials in `src/api/apiConstants.js`:
 
```js
export const APP_ID = "your_app_id"
export const APP_KEY = "your_app_key"
```
 
```bash
# Start the dev server
npm run dev
```

Open [http://localhost:5173](http://localhost:5173) in your browser.

## 📁 Project Structure

```
recipe/
├── src/
│   ├── api/
│   │   ├── axios.js            # Axios instance with baseURL config
│   │   └── apiConstants.js     # Edamam APP_ID and APP_KEY
│   ├── components/
│   │   ├── common/             # Navbar, Header, Footer, Loader, Searchbar, Sliders...
│   │   └── recipe/             # RecipeItem, RecipeList
│   ├── views/                  # Page-level components
│   │   ├── home/               # HomePage
│   │   ├── recipe/             # RecipeListPage, RecipeSinglePage, RecipeSearchPage
│   │   ├── type/               # TypeListPage
│   │   └── error/              # 404 ErrorPage
│   ├── redux/
│   │   ├── store/              # recipesSlice, typesSlice, store.js
│   │   └── utils/              # recipeUtils, typeUtils (createAsyncThunk)
│   ├── layouts/
│   │   └── BaseLayout.jsx      # Shared layout with Navbar + Footer
│   └── utils/                  # helpers, images, status constants, scrollToTop
```

## 📝 Notes
 
- Requires a free Edamam API account for credentials
- The Edamam free tier has rate limits — heavy usage may return 429 errors
 
## 📄 License
 
This project is open source and available under the [MIT License](LICENSE).
 
## 👤 Author
 
**Luan Neumann**
 
- GitHub: [@Luan-Neumann-Dev](https://github.com/Luan-Neumann-Dev)
- LinkedIn: [luan-neumann-dev](https://www.linkedin.com/in/luan-neumann-dev/)
