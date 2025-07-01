---

# 🎯 Hub200 Website (Made with Django)

A responsive, multipage website built with Django, designed to showcase content and provide interactive user engagement. Built by Abbas‑AG.

---
youtube video: https://www.youtube.com/watch?v=OQW9b1F8btQ

## 🚀 Features

* **User Authentication**

  * Registration and login functionality for site access
  * Standard Django auth system

* **Home Page & About Section**

  * Features a hero banner
  * Includes an About page with static content

* **Services Page**

  * Lists available services with title, brief description, and icon/image

* **Contact Page**

  * Contact form for users to submit inquiries
  * Form data is sent to site administrators via email

* **Dynamic Navigation**

  * Navbar updates based on user login status
  * Includes “Login”, “Register”, and “Logout” links

* **Admin Panel (Django Admin)**

  * Manage services, contact messages, and site settings
  * Full CRUD support for service entries

* **Static & Media Management**

  * Uses Django’s static files system for CSS and JS
  * Handles media assets (images/icons) with proper configuration

---

## 🧩 Installation

```bash
git clone https://github.com/Abbas-AG/hub200-website-made-with-django.git
cd hub200-website-made-with-django

python -m venv venv
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

pip install -r requirements.txt
python manage.py migrate

python manage.py createsuperuser
python manage.py runserver
```

Access the app at `http://127.0.0.1:8000/` and the admin panel at `http://127.0.0.1:8000/admin/`.

---

## 📂 Project Structure

```
hub200-website/
├── manage.py
├── requirements.txt
├── core/
│   ├── models.py          # Service, ContactMessage models
│   ├── views.py           # Views for pages and form handling
│   ├── urls.py            # Routing
│   ├── templates/         # Templates (base, home, service, contact, auth)
│   └── static/            # CSS, JS, images
└── hub200_website/        # Django project settings
    └── settings.py        # Static/media config, email settings
```

---

## ⚙️ Configuration Notes

* **Email setup**
  Configure SMTP (e.g., Gmail, SendGrid) in `settings.py` to enable contact form emails (`EMAIL_BACKEND`, `EMAIL_HOST`, etc.).

* **Static & Media Files**
  Ensure `STATIC_URL` and `MEDIA_URL` are properly configured. Run `python manage.py collectstatic` in production.

* **Admin Access**
  Use the created superuser to log into the Django admin panel and manage content.

---

## ✅ Usage Steps

1. Sign up or log into the site
2. Browse home, about, and services pages
3. Fill out the contact form to send a message to the admin
4. Admin users can manage Services and Contact Submissions via the admin panel

---

## 📢 Contributing

* Open issues or PRs for feature requests or bug fixes
* Adhere to PEP 8 style and include comments
* Ensure static and media files are properly referenced

---

## ℹ️ Contact

If you have questions or suggestions, feel free to open an issue or reach out via Telegram: @ENG_AG.

Enjoy building with Django 🎉
