интернет-магазин

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
- `cd my-project` - путь 
- `npm install` - установка 
- `npm run dev` - запуск
- `http://localhost:5173` - ссылка


## 3.3. Запуск бэкенда
- `npm i ` - установка
- `npm run dev ` - запуск 

## 4.1. Пример: мы запрашиваем список продуктов через Redux-thunk
``` 
   export const fetchProducts = () => async (dispatch) => {
    dispatch({ type: "PRODUCTS_LOADING" });
    try {
      const res = await fetch("http://localhost:4000/products");
      const data = await res.json();
      dispatch({ type: "PRODUCTS_SUCCESS", payload: data });
    } catch (e) {
      dispatch({ type: "PRODUCTS_ERROR", payload: e.message });
    }
  };
```

## 4.2. React hook 
``` 
const { register, handleSubmit } = useForm();

``` 

## 5. Структура 

```  my-project/
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
```


## 6. Технические требования

- Фреймворк: React 18+
- Маршрутизация: react-router-dom v6+
- Состояние: Redux + redux-thunk
- Формы: react-hook-form
- Node.js: версия 17+
- ОС: Windows / macOS / Linux

 ## 7.Автор
 Авдиенко Егор Сергеевич

 ## 8. Тестирование и обратная связь

5 КТ было проведено тестирование проекта «Магазин для сада».

### Проведенные типы тестирования:
- Функциональное
- Пользовательское
- UI/UX
- Тестирование форм
- Тестирование API

### Подготовленные документы находятся в разделе с README:
- `test_plan.md` — план тестирования  
- `test_report.md` — таблица результатов тестов  
- `feedback_summary.md` — анализ отзывов пользователей  
- `issues.md` — найденные ошибки и улучшения  

### Основные найденные проблемы:
- Некорректное удаление товаров из корзины  
- Ошибки адаптивной верстки  

### Полученная обратная связь :
оценки положительные (4.2/5), некоториые пользователи предложили улучшить адаптивность и добавить фильтры.



 ## 9.Контакты

 Email: egoregor641618@gmail.com
 tg: @xrngo


 
