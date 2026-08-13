<div align="center">

# ✅ Taski

**Task planner with a Django REST API and a React single-page frontend**

![Python](https://img.shields.io/badge/Python-3.12-3776AB?logo=python&logoColor=white) ![Django](https://img.shields.io/badge/Django-5.1-092E20?logo=django&logoColor=white) ![DRF](https://img.shields.io/badge/DRF-3.15-A30000?logo=django&logoColor=white) ![React](https://img.shields.io/badge/React-SPA-61DAFB?logo=react&logoColor=black) [![CI](https://github.com/ikovalll/taski/actions/workflows/ci.yml/badge.svg)](https://github.com/ikovalll/taski/actions/workflows/ci.yml) ![License](https://img.shields.io/badge/license-MIT-lightgrey)

[**English**](README.md) · [Русский](README.ru.md)

</div>

---

## 📖 About

A small task management application. The backend is a Django REST Framework API over a single `Task` model; the frontend is a React SPA that talks to it through CORS-enabled endpoints. The project is the starting point of the infrastructure track — the containerised version lives in [taski-docker](https://github.com/ikovalll/taski-docker).

---

## ✨ Features

- **Tasks** — create, edit, complete and delete via REST API
- **React SPA** — task list, tabs and an edit modal
- **CORS** — frontend and backend run as separate services
- **Admin site** for managing tasks

---

## 🛠 Tech Stack

| Layer | Technologies |
|---|---|
| **Backend** | Python 3.12, Django 5.1, Django REST Framework |
| **Frontend** | React SPA |
| **Database** | SQLite |
| **Integration** | django-cors-headers |
| **Quality** | flake8, GitHub Actions |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.12+
- Node.js 18+

### Backend

```bash
git clone git@github.com:ikovalll/taski.git
cd taski/backend

python3.12 -m venv venv
source venv/bin/activate
pip install -r requirements.txt

python manage.py migrate
python manage.py runserver
```

### Frontend

```bash
cd frontend
npm install
npm start
```

- API: `http://127.0.0.1:8000/api/`
- App: `http://localhost:3000/`

---

## 📁 Project Structure

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

Every push and pull request runs a GitHub Actions workflow that installs dependencies and lints the code with `flake8` using the repository config.

---

## 📄 License

Distributed under the MIT License. See [LICENSE](LICENSE) for details.

---

## 👤 Author

**Ilia Kovalenko**

[GitHub](https://github.com/ikovalll) · [Telegram](https://t.me/ikovalll) · [LinkedIn](https://www.linkedin.com/in/ikovalll/)
