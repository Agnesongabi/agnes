# Agnes Ongabi - Portfolio Website

A modern, responsive portfolio website built with Django to showcase my projects, skills, and professional experience.

## 🌟 Features

- **Responsive Design** - Optimized for desktop, tablet, and mobile devices
- **Project Showcase** - Interactive gallery of my development projects
- **Skills & Technologies** - Comprehensive overview of my technical expertise
- **About Me** - Professional background and personal story
- **Contact Form** - Direct communication with form validation
- **Admin Panel** - Easy content management through Django admin
- **Blog Section** - Share insights and technical articles
- **SEO Optimized** - Meta tags and structured data for better search visibility

## 🚀 Live Demo

Visit my portfolio: [Your Portfolio URL]

## 🛠️ Technologies Used

### Backend
- **Django 4.x** - Python web framework
- **Python 3.9+** - Programming language
- **SQLite/PostgreSQL** - Database
- **Django REST Framework** - API development (if applicable)

### Frontend
- **HTML5 & CSS3** - Structure and styling
- **JavaScript** - Interactive functionality
- **Bootstrap 5** - CSS framework
- **Font Awesome** - Icons
- **AOS (Animate On Scroll)** - Scroll animations

### Deployment & DevOps
- **Gunicorn** - WSGI HTTP Server
- **Nginx** - Web server (production)
- **Docker** - Containerization (optional)
- **Git** - Version control

## 📋 Prerequisites

Before running this project, make sure you have:

- Python 3.9 or higher
- pip (Python package manager)
- Git
- Virtual environment tool (venv or virtualenv)

## ⚡ Quick Start

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/agnes-ongabi-portfolio.git
cd agnes-ongabi-portfolio
```

### 2. Create Virtual Environment
```bash
# On Windows
python -m venv venv
venv\Scripts\activate

# On macOS/Linux
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Environment Configuration
Create a `.env` file in the root directory:
```env
SECRET_KEY=your-secret-key-here
DEBUG=True
DATABASE_URL=sqlite:///db.sqlite3
EMAIL_HOST_USER=your-email@gmail.com
EMAIL_HOST_PASSWORD=your-app-password
```

### 5. Database Setup
```bash
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser
```

### 6. Load Sample Data (Optional)
```bash
python manage.py loaddata fixtures/sample_data.json
```

### 7. Run Development Server
```bash
python manage.py runserver
```

Visit `http://127.0.0.1:8000` to view the portfolio.

## 📁 Project Structure

```
agnes-ongabi-portfolio/
│
├── portfolio/                 # Main Django project
│   ├── __init__.py
│   ├── settings.py           # Project settings
│   ├── urls.py              # Main URL configuration
│   └── wsgi.py              # WSGI configuration
│
├── apps/
│   ├── core/                # Core functionality
│   │   ├── models.py        # Database models
│   │   ├── views.py         # View functions
│   │   ├── urls.py          # App URLs
│   │   └── admin.py         # Admin configuration
│   │
│   ├── projects/            # Project showcase app
│   ├── blog/                # Blog functionality
│   └── contact/             # Contact form app
│
├── static/                  # Static files
│   ├── css/
│   ├── js/
│   ├── img/
│   └── fonts/
│
├── templates/               # HTML templates
│   ├── base.html
│   ├── home.html
│   ├── about.html
│   ├── projects.html
│   └── contact.html
│
├── media/                   # User uploaded files
├── requirements.txt         # Python dependencies
├── manage.py               # Django management script
├── .env.example            # Environment variables template
├── .gitignore             # Git ignore file
└── README.md              # This file
```

## 🎨 Customization

### Adding New Projects
1. Access the Django admin panel at `/admin/`
2. Navigate to Projects section
3. Add new project with:
   - Title and description
   - Technologies used
   - GitHub repository link
   - Live demo URL
   - Project screenshots

### Updating Personal Information
- Edit the About model in Django admin
- Update social media links in `settings.py`
- Modify contact information in the Contact app

### Styling Changes
- Main styles are in `static/css/main.css`
- Bootstrap customizations in `static/css/custom.css`
- Color scheme variables at the top of CSS files

## 📧 Contact Form Setup

To enable the contact form functionality:

1. Configure email settings in `.env`:
```env
EMAIL_HOST=smtp.gmail.com
EMAIL_PORT=587
EMAIL_USE_TLS=True
EMAIL_HOST_USER=your-email@gmail.com
EMAIL_HOST_PASSWORD=your-app-password
```

2. For Gmail, generate an app-specific password
3. Update `ADMINS` setting in `settings.py`

## 🚀 Deployment

### Using Heroku
1. Install Heroku CLI
2. Create `Procfile`:
```
web: gunicorn portfolio.wsgi:application
```
3. Deploy:
```bash
heroku create your-portfolio-name
git push heroku main
heroku run python manage.py migrate
```

### Using DigitalOcean/AWS
1. Set up server with Python and Nginx
2. Configure Gunicorn and systemd service
3. Set up SSL certificate with Let's Encrypt
4. Configure environment variables for production

## 🧪 Testing

Run the test suite:
```bash
python manage.py test
```

Run with coverage:
```bash
pip install coverage
coverage run --source='.' manage.py test
coverage report
coverage html
```

## 📈 Performance

- **Lighthouse Score**: 95+ (Performance, Accessibility, Best Practices, SEO)
- **Load Time**: < 2 seconds
- **Mobile Responsive**: Yes
- **Cross-browser Compatible**: Chrome, Firefox, Safari, Edge

## 🤝 Contributing

While this is a personal portfolio, I welcome suggestions and improvements:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit changes (`git commit -am 'Add new feature'`)
4. Push to branch (`git push origin feature/improvement`)
5. Create a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Contact

**Agnes Ongabi**
- Portfolio: [Your Portfolio URL]
- Email: your.email@example.com
- LinkedIn: [Your LinkedIn Profile]
- GitHub: [Your GitHub Profile]
- Twitter: [@yourusername]

## 🙏 Acknowledgments

- Django community for the excellent framework
- Bootstrap team for the responsive CSS framework
- Font Awesome for the beautiful icons
- Unsplash for stock photography
- All the open-source contributors who made this possible

---

⭐ **If you found this project helpful, please consider giving it a star!**

---

*Last updated: September 2025*