# ReactComponentsFunc 🧩

**ReactComponentsFunc** — это демонстрационный проект на React, реализующий функциональный компонент для отображения карточки товара интернет-магазина. Проект создан с использованием Vite и демонстрирует базовые принципы работы с функциональными компонентами и пропсами.

## 🛠 Технологический стек

- **React 18** — библиотека для построения пользовательских интерфейсов
- **Vite** — инструмент сборки и разработки
- **JavaScript (ES6+)** — язык программирования
- **CSS** — стилизация компонентов
- **ESLint** — линтинг кода

## 🚀 Установка и запуск

1. **Клонируйте репозиторий:**
   ```bash
   git clone https://github.com/your-username/ReactComponentsFunc.git
   cd ReactComponentsFunc
   ```

2. **Установите зависимости:**
   ```bash
   npm install
   ```

3. **Запустите сервер разработки:**
   ```bash
   npm run dev
   ```

4. **Откройте в браузере:**
   ```
   http://localhost:5173
   ```

## 💻 Примеры использования

### Основной компонент `ShopItemFunc`

```jsx
// src/App.jsx
import ShopItemFunc from './components/ShopItemFunc';

const item = {
  brand: 'Nike',
  title: 'Air Max 270',
  description: 'Кроссовки с амортизацией',
  descriptionFull: 'Модель с максимальным комфортом...',
  price: 150,
  currency: '€'
};

function App() {
  return (
    <div className="container">
      <ShopItemFunc item={item} />
    </div>
  );
}
```

### Компонент `ShopItemFunc`

```jsx
// src/components/ShopItemFunc.jsx
function ShopItemFunc({ item }) {
  return (
    <div className="shop-item">
      <h2>{item.brand}</h2>
      <h3>{item.title}</h3>
      <p>{item.description}</p>
      <p className="price">{item.price} {item.currency}</p>
    </div>
  );
}

export default ShopItemFunc;
```

## 📁 Структура проекта

```
ReactComponentsFunc/
├── public/
│   └── vite.svg
├── src/
│   ├── assets/
│   │   └── react.svg
│   ├── components/
│   │   ├── index.js
│   │   └── ShopItemFunc.jsx
│   ├── img/
│   │   ├── item-black.jpg
│   │   └── item-blue.jpg
│   ├── App.css
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── index.html
├── package.json
├── package-lock.json
├── vite.config.js
├── eslint.config.js
└── README.md
```

## 📄 Лицензия

Этот проект распространяется под лицензией **MIT**. Подробнее см. в файле [LICENSE](LICENSE).