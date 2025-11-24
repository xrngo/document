# IE-Fe-Shop — Учебный интернет-магазин (React + Redux)

## 1. Название проекта
Магазин для сада

## 2. Описание проекта
Данный проект представляет собой учебное веб-приложение интернет-магазина для садоводов.  
Проект предназначен для отработки моих навыков с :

- React и компонентной архитектурой  
- React Router  
- Redux и redux-thunk  
- React Hook Form  
- Структурированием проекта по современным фронтенд-паттернам  

Приложение включает страницы каталога, товара и корзины, а также взаимодействует с локальным бэкендом.

## 3. Установка и запуск
1.cd my-project
2.npm install
3.npm run dev 
4.http://localhost:5173


## 3.3. Запуск бэкенда
### `npm i `
### `npm run dev `

## 4. Пример: мы запрашиваем список продуктов через Redux-thunk

##    export const fetchProducts = () => async (dispatch) => {
##     dispatch({ type: "PRODUCTS_LOADING" });
##      try {
##        const res = await fetch("http://localhost:4000/products");
##        const data = await res.json();
##        dispatch({ type: "PRODUCTS_SUCCESS", payload: data });
##      } catch (e) {
##        dispatch({ type: "PRODUCTS_ERROR", payload: e.message });
##      }
##    };


## 5. Структура 

  my-project/
  ├─ public/
  ├─ src/
  │  ├─ assets/              
  │  ├─ components/
  │  │  ├─ Button/
  │  │  │   ├─ Button.jsx
  │  │  │   └─ Button.module.css
  │  │  ├─ CategoryCard/
  │  │  │   ├─ CategoryCard.jsx
  │  │  │   └─ CategoryCard.module.css
  │  │  └─ ProductCard/
  │  │      ├─ ProductCard.jsx
  │  │      └─ ProductCard.module.css
  │  │
  │  ├─ pages/
  │  │  ├─ HomePage/
  │  │  │   ├─ HomePage.jsx
  │  │  │   └─ HomePage.module.css
  │  │  └─ CartPage/
  │  │      ├─ CartPage.jsx
  │  │      └─ CartPage.module.css
  │  │
  │  ├─ store/
  │  │  ├─ slices/
  │  │  │   ├─ cartSlice.js
  │  │  │   ├─ categoriesSlice.js
  │  │  │   └─ productsSlice.js
  │  │  ├─ index.js
  │  │  └─ store.js
  │  │
  │  ├─ styles/
  │  │  └─ global.css
  │  │
  │  ├─ App.jsx
  │  ├─ main.jsx
  │  └─ index.css
  │
  ├─ package.json
  ├─ vite.config.js
  ├─ .gitignore
  └─ README.md



## 6. Технические требования

- Фреймворк: React 18+
- Маршрутизация: react-router-dom v6+
- Состояние: Redux + redux-thunk
- Формы: react-hook-form
- Node.js: версия 17+
- ОС: Windows / macOS / Linux
