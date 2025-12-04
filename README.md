# KYU-RESOURCE-SHARING-PLATFORM
KyHub Connect: Kyambogo University's smart campus platform for sharing academic resources &amp; booking study spaces. Built with Django/React.
# 📚 KyHub Connect - Campus Academic Resource Platform

**A peer-to-peer platform for Kyambogo University students to share academic resources and manage study spaces**

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Django](https://img.shields.io/badge/Django-4.0-green.svg)](https://www.djangoproject.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-13-blue.svg)](https://www.postgresql.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 🎯 Problem Statement
Kyambogo University students face two major challenges:
1. **Fragmented Academic Resources:** Past papers, lecture notes, and study materials are scattered across WhatsApp groups, personal drives, and physical copies
2. **Inefficient Study Space Management:** Students waste valuable time searching for available study rooms and spaces on campus

## ✨ Solution
KyHub Connect provides a unified platform where students can:
- **Share & Discover** quality academic resources
- **Earn Reward Points** for contributing materials
- **Book & Find** available study spaces
- **Collaborate** with peers studying similar courses

## 🚀 Features

### **Phase 1: Resource Sharing System (Current Focus)**
✅ **User Authentication** - Secure login with Kyambogo email verification  
✅ **Resource Upload/Download** - Support for PDFs, DOCs, PPTs with preview  
✅ **Smart Categorization** - Organized by course code, faculty, and year  
✅ **Points & Reward System** - Earn points for uploads, spend for downloads  
✅ **Quality Control** - Peer ratings and moderator approval system  
✅ **Advanced Search** - Filter by course, year, resource type, rating  

### **Phase 2: Study Space Integration (Coming Soon)**
🔜 Real-time room availability tracking  
🔜 QR-based check-in system  
🔜 Room booking and reservation  
🔜 Integration with university timetable  

## 🛠️ Technology Stack

**Backend:**
- Python 3.9+
- Django 4.0+
- Django REST Framework (for APIs)
- PostgreSQL 13+

**Frontend:**
- HTML5, CSS3, JavaScript
- Bootstrap 5 for responsive design
- Chart.js for analytics dashboards

**Services & APIs:**
- AWS S3 / DigitalOcean Spaces for file storage
- SendGrid for email notifications
- Africa's Talking SMS API (future)

**DevOps:**
- Docker for containerization
- GitHub Actions for CI/CD
- Heroku / DigitalOcean for deployment

## 📦 Installation & Setup

### Prerequisites
- Python 3.9 or higher
- PostgreSQL 13+
- pip (Python package manager)
- Git

### Local Development Setup
```bash
# 1. Clone the repository
git clone https://github.com/YOUR_USERNAME/kyhub-connect.git
cd kyhub-connect

# 2. Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Configure environment variables
cp .env.example .env
# Edit .env with your database credentials

# 5. Run migrations
python manage.py migrate

# 6. Create superuser
python manage.py createsuperuser

# 7. Run development server
python manage.py runserver
