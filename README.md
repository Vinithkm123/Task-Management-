Below is a **clean, simple, copy-paste READY `README.md`** for your project.
It is **final-year / VTU / GitHub friendly** and matches **exactly your running code**.

---

```markdown
# 📊 Data Visualization Dashboard (Full Stack)

A simple **full-stack web application** built using **Django REST Framework** and **React** to visualize data using SVG charts.

---

## 🚀 Features

- Django REST API backend
- React frontend (Vite)
- SVG-based bar chart visualization
- MySQL database
- No Redux
- No external UI libraries
- Clean and minimal architecture

---

## 🧱 Tech Stack

### Backend
- Python 3
- Django
- Django REST Framework
- MySQL
- django-cors-headers

### Frontend
- React 18
- Vite
- Tailwind CSS
- JavaScript (ES6)

---

## 📁 Project Structure

```

fullstack-app/
│
├── backend/
│   ├── backend/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── ...
│   ├── api/
│   │   ├── models.py
│   │   ├── serializers.py
│   │   ├── views.py
│   │   ├── urls.py
│   └── manage.py
│
└── frontend/
├── src/
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
└── tailwind.config.js

````

---

## ⚙️ Backend Setup (Django)

### 1️⃣ Create Virtual Environment
```bash
cd backend
python -m venv venv
venv\Scripts\activate
````

### 2️⃣ Install Dependencies

```bash
pip install django djangorestframework mysqlclient django-cors-headers
```

### 3️⃣ Run Migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 4️⃣ Create Superuser

```bash
python manage.py createsuperuser
```

### 5️⃣ Start Server

```bash
python manage.py runserver
```

### 6️⃣ Test API

Open browser:

```
http://127.0.0.1:8000/api/data/
```

---

## 🗄️ Database Configuration

Configured in `settings.py`:

```python
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.mysql',
        'NAME': 'dashboard_db',
        'USER': 'root',
        'PASSWORD': 'password',
        'HOST': 'localhost',
        'PORT': '3306',
    }
}
```

---

## 🖥️ Frontend Setup (React)

### 1️⃣ Install Dependencies

```bash
cd frontend
npm install
```

### 2️⃣ Run Frontend

```bash
npm run dev
```

Open:

```
http://localhost:5173
```

---

## 📊 Visualization Output

* Data fetched from Django REST API
* Rendered as SVG bar chart
* Dynamic height based on database values

---

## 🔐 Admin Panel

```
http://127.0.0.1:8000/admin/
```

Add data using **DataPoint model**:

* label (string)
* value (integer)

---

## 🔄 API Endpoint

| Method | Endpoint     | Description              |
| ------ | ------------ | ------------------------ |
| GET    | `/api/data/` | Fetch visualization data |

---

## 🧪 Sample API Response

```json
[
  { "id": 1, "label": "A", "value": 120 },
  { "id": 2, "label": "B", "value": 200 }
]
```

---

## 📌 Future Enhancements

* Authentication (JWT)
* Advanced charts (D3.js)
* Dashboard filters
* Deployment (AWS / Render)

---


