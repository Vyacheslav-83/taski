<div align="center">

# ✅ Taski

**Планировщик задач: Django REST API и одностраничный фронтенд на React**

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-5.1-092E20?logo=django&logoColor=white) ![DRF](https://img.shields.io/badge/DRF-3.15-A30000?logo=django&logoColor=white) ![React](https://img.shields.io/badge/React-SPA-61DAFB?logo=react&logoColor=black) [![CI](https://github.com/ikovalll/taski/actions/workflows/ci.yml/badge.svg)](https://github.com/ikovalll/taski/actions/workflows/ci.yml) ![License](https://img.shields.io/badge/license-MIT-lightgrey)

[English](README.md) · [**Русский**](README.ru.md)

</div>

---

## 📖 О проекте

Небольшое приложение для планирования задач. Бэкенд — API на Django REST Framework поверх одной модели `Task`, фронтенд — React SPA, который обращается к нему через CORS. Это отправная точка инфраструктурного трека — контейнеризированная версия лежит в [taski-docker](https://github.com/ikovalll/taski-docker).

---

## ✨ Возможности

- **Задачи** — создание, редактирование, отметка выполнения и удаление через REST API
- **React SPA** — список задач, вкладки и модальное окно редактирования
- **CORS** — фронтенд и бэкенд работают как отдельные сервисы
- **Админка** для управления задачами

---

## 🛠 Стек технологий

| Слой | Технологии |
|---|---|
| **Бэкенд** | Python 3.12, Django 5.1, Django REST Framework |
| **Фронтенд** | React SPA |
| **База данных** | SQLite |
| **Интеграция** | django-cors-headers |
| **Качество кода** | flake8, GitHub Actions |

---

## 🚀 Запуск

### Требования

- Python 3.12+
- Node.js 18+

### Бэкенд

```bash
git clone git@github.com:ikovalll/taski.git
cd taski/backend

python3.12 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

python manage.py migrate
python manage.py runserver
```

### Фронтенд

```bash
cd frontend
npm install
npm start
```

- API: `http://127.0.0.1:8000/api/`
- Приложение: `http://localhost:3000/`

---

## 📁 Структура проекта

```
taski/
├── backend/
│   ├── api/               # Task model, serializers, views
│   ├── backend/           # project settings
│   └── requirements.txt
└── frontend/              # React SPA
    └── src/components/    # TabList, Task, TaskEditModal
```

---

## ⚙️ CI

На каждый push и pull request запускается workflow GitHub Actions: устанавливает зависимости и проверяет код `flake8` по конфигу репозитория.

---

## 📄 Лицензия

Проект распространяется под лицензией MIT. Подробности — в файле [LICENSE](LICENSE).

---

## 👤 Автор

**Илья Коваленко**

[GitHub](https://github.com/ikovalll) · [Telegram](https://t.me/ikovalll) · [LinkedIn](https://www.linkedin.com/in/ikovalll/)
