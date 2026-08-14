# 🚀 Extera Plugins Catalog

<div align="center">

![Preview](https://img.shields.io/badge/Telegram-WebApp-26A5E4?style=for-the-badge&logo=telegram)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Active-success?style=for-the-badge)

**Premium Telegram Mini App для каталога плагинов, модулей и приложений**

[Demo](#) • [Features](#-features) • [Installation](#-installation) • [Usage](#-usage)

</div>

---

## ✨ Features

### 🎨 **Современный UI/UX**
- **Glassmorphism дизайн** — полупрозрачные карточки с эффектом размытия
- **Ambient анимации** — плавные градиентные фоны с аврора-эффектом
- **Микро-взаимодействия** — hover-эффекты, ripple animations, параллакс иконок
- **Адаптивность** — идеально работает на всех устройствах

### ⚡ **Производительность**
- **Оптимизированные анимации** — 60 FPS благодаря CSS transforms
- **Ленивая загрузка** — skeleton screens при переключении страниц
- **Debounce & Throttle** — умная обработка событий поиска и скролла

### 🔧 **Функционал**
| Функция | Описание |
|---------|----------|
| 📑 **Пагинация** | Удобная навигация по страницам с кнопками |
| 🔍 **Поиск** | Мгновенный поиск по названию и описанию |
| 🔄 **Свайпы** | Горизонтальные свайпы для переключения страниц |
| 📋 **Копирование** | Копирование ссылки в один клик |
| 🌙 **Dark Mode** | Глубокая тёмная тема с неоновыми акцентами |
| 🔐 **Secret Mode** | Скрытый раздел (7 кликов по заголовку) |

### 📱 **Telegram Integration**
- ✅ Haptic Feedback при взаимодействиях
- ✅ Автоматическое раскрытие WebApp
- ✅ Нативная кнопка «Назад» для секретного раздела
- ✅ Адаптация под тему Telegram

---

## 🛠️ Installation

### 1. Клонирование репозитория
```bash
git clone https://github.com/yourusername/extera-catalog.git
cd extera-catalog
```

### 2. Размещение файлов
Разместите `index.html` на любом хостинге:
- **GitHub Pages** (бесплатно)
- **Vercel / Netlify** (бесплатно)
- **Свой сервер** (nginx/Apache)

### 3. Настройка Telegram Bot
```javascript
// В @BotFather создайте бота и привяжите WebApp
/newapp → укажите URL вашего хостинга
```

---

## 📖 Usage

### Навигация
1. **Вкладки** — переключайтесь между плагинами, модулями, приложениями и ботами
2. **Поиск** — начните вводить название для фильтрации
3. **Свайп** ← → — листайте страницы жестом
4. **Кнопки** — откройте ссылку или скопируйте её

### Secret Mode 🤫
Нажмите **7 раз** на заголовок «КАТАЛОГ» за 2 секунды для доступа к скрытому разделу.

---

## 🎯 Customization

### Добавление нового элемента
Откройте `index.html` и найдите объект `DATA`:

```javascript
const DATA = {
    plugins: [
        { 
            name: "YourPlugin", 
            url: "https://t.me/yourchannel/123", 
            desc: "Описание плагина" 
        },
        // ... другие элементы
    ],
    // modules, apps, bots...
};
```

### Изменение цветовой схемы
В секции `<style>` измените CSS переменные:

```css
:root {
    --plugin: #00f2ff;    /* Основной акцент */
    --module: #ff9500;    /* Модули */
    --app: #ff2d55;       /* Приложения */
    --bot: #bd00ff;       /* Боты */
}
```

### Добавление кастомной иконки
Найдите объект `ICONS` и добавьте SVG:

```javascript
ICONS.plugins['YourPlugin'] = `
    <svg viewBox="0 0 100 100" xmlns="http://www.w3.org/2000/svg">
        <!-- Ваш SVG код -->
    </svg>
`;
```

---

## 📊 Structure

```
extera-catalog/
├── index.html          # Основное приложение (HTML + CSS + JS)
└── README.md           # Документация
```

**Всего 1 файл!** Весь код находится в `index.html` для простоты развёртывания.

---

## 🚀 Performance

| Metric | Value |
|--------|-------|
| Load Time | < 1s |
| First Paint | ~200ms |
| Animations | 60 FPS |
| Bundle Size | ~65 KB |

---

## 📝 License

MIT License — свободно используйте и модифицируйте.

---

## 👨‍💻 Author

Created with ❤️ for the Extera Community

---

<div align="center">

**Enjoy the Catalog!** 🎉

[⬆ Back to Top](#-extera-plugins-catalog)

</div>

