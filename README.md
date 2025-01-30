# PRINT-HONEST-SIGN

## 📝 О проекте
**PRINT-HONEST-SIGN** — это клиент-серверное приложение, предназначенное для добавления, хранения, учета и реализации честного знака. Проект разделен на две части: **backend** (серверная часть, Node.js + Express) и **frontend** (клиентская часть, React). Также включены файлы конфигурации и скрипты для автоматизации процессов.

---

## 🛠️ Общая структура

### Backend (серверная часть)
Находится в папке `backend`, включает:
- **config/connectdb.js**: Настройка подключения к базе данных.
- **controllers/**: Обработчики API:
  - `infoHSController.js`
  - `kyzController.js`
  - `printedHSController.js`
- **models/**: Отсутствует, но предполагается наличие моделей данных.
- **utils/pdfProcessor.js**: Обработка PDF-документов.
- **server.js**: Основной файл сервера, запускает API.
  
![Node.js](https://img.shields.io/badge/Node.js-16-green?logo=node.js)
![Express](https://img.shields.io/badge/Express-4.17-blue?logo=express)

### Frontend (клиентская часть)
Находится в папке `frontend`, включает:
- **public/**: Статические файлы (иконка, HTML, манифест).
- **src/**: Исходный код:
  - **Компоненты (components/)**:
    - `AdminPanel.js`: Панель администратора.
    - `Error.js`: Обработка ошибок.
    - `LoadScreen.js`: Загрузочный экран.
    - `ReportGenerator.js`: Генерация отчетов.
    - `SignDisplay.js`: отображение подписей и документов.
  - **CSS-стили (css/)**.
  - **JSON (json/)**: Возможно, содержит статические данные.
  - **Основные файлы (App.js, index.js)**: Основа React-приложения.
  
![React](https://img.shields.io/badge/React-18-blue?logo=react)
![Vite](https://img.shields.io/badge/Vite-2.9-purple?logo=vite)

### Дополнительные файлы
- **.env**: Хранит переменные окружения.
- **.gitignore**: Файлы, игнорируемые Git.
- **.bat и .vbs файлы**: автоматизация процессов (например, запуск сервера, генерация отчетов, обработка данных).

---

## 🚀 Функционал

- 🖨 **Добавление и хранение честных знаков**
- 📊 **Учет и управление данными**
- 📄 **Обработка и работа с PDF-документами**
- 🔍 **Генерация отчетов**
- ⚙️ **Автоматизация процессов**

---

## 🛠️ Технологии

### Backend
![Node.js](https://img.shields.io/badge/Node.js-16-green?logo=node.js)
![Express](https://img.shields.io/badge/Express-4.17-blue?logo=express)
![JWT](https://img.shields.io/badge/JWT-Auth-orange?logo=jsonwebtokens)
![Multer](https://img.shields.io/badge/Multer-File_Upload-purple?logo=multer)

### Frontend
![React](https://img.shields.io/badge/React-18-blue?logo=react)
![Vite](https://img.shields.io/badge/Vite-2.9-purple?logo=vite)
![Redux](https://img.shields.io/badge/Redux-Toolkit-yellow?logo=redux)

### База данных
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-DB-brightgreen?logo=postgresql)

---

## 📦 Установка и запуск

### 🔧 Backend

1. Перейдите в директорию `backend`:
    ```sh
    cd backend
    ```
2. Установите зависимости:
    ```sh
    npm install
    ```
3. Запустите сервер:
    ```sh
    npm start
    ```

### 🌐 Frontend

1. Перейдите в директорию `frontend`:
    ```sh
    cd frontend
    ```
2. Установите зависимости:
    ```sh
    npm install
    ```
3. Запустите приложение в режиме разработки:
    ```sh
    npm run dev
    ```

---

## 📌 API Эндпоинты

### 📍 Аутентификация

| Метод | URL                  | Описание                       |
| ----- | -------------------- | ------------------------------ |
| POST  | `/api/auth/register` | Регистрация пользователя       |
| POST  | `/api/auth/login`    | Авторизация и получение токена |

### 📍 Честные знаки

| Метод  | URL              | Описание                             |
| ------ | ---------------- | ------------------------------------ |
| GET    | `/api/honestsigns`     | Получить все честные знаки                   |
| POST   | `/api/honestsigns`     | Создать новый честный знак (требуется токен) |
| PUT    | `/api/honestsigns/:id` | Обновить честный знак (требуется токен)      |
| DELETE | `/api/honestsigns/:id` | Удалить честный знак (требуется токен)       |

---

## 📊 Вывод
Приложение **PRINT-HONEST-SIGN** представляет собой клиент-серверное приложение с:
- **Бэкендом на Node.js + Express**, работающим с базой данных и PDF.
- **Фронтендом на React**, ориентированным на отчеты и визуализацию данных.
- **Автоматизированными процессами** через `.bat` и `.vbs`.

---
