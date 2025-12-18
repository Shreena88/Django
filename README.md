# Tweet App - Django Social Media Application

A modern Twitter-like social media application built with Django, featuring CRUD operations and a beautiful responsive design.

## 📁 Project Structure

```
├── project/
│   └── tweet/                # Tweet App Django Project
│       ├── first/            # Main tweet application
│       │   ├── models.py     # Tweet model
│       │   ├── views.py      # Tweet CRUD views
│       │   ├── forms.py      # Tweet forms
│       │   ├── urls.py       # URL routing
│       │   ├── admin.py      # Admin configuration
│       │   └── templates/    # HTML templates
│       │       ├── index.html
│       │       ├── tweet_list.html
│       │       ├── tweet_form.html
│       │       └── tweet_confirm_delete.html
│       ├── templates/        # Base templates
│       │   └── layout.html   # Main layout template
│       ├── media/            # Uploaded images
│       ├── tweet/            # Project settings
│       └── manage.py
└── README.md
```

---

## 🐦 Tweet App

A Twitter-like social media application with CRUD operations and modern UI.

### Features
- **Tweet Management**: Create, read, update, delete tweets
- **Image Upload**: Attach photos to tweets
- **User Authentication**: Tweet ownership and permissions
- **Responsive Design**: Purple gradient theme with card layouts
- **Modern UI**: Bootstrap 5 with custom styling

### Technologies Used
- Django 5.2.7
- Bootstrap 5.3.8
- Font Awesome icons
- SQLite database
- Custom CSS with gradients

### Setup Instructions

1. **Navigate to Tweet App**
   ```bash
   cd project/tweet
   ```

2. **Install Dependencies**
   ```bash
   pip install django pillow
   ```

3. **Run Migrations**
   ```bash
   py manage.py makemigrations
   py manage.py migrate
   ```

4. **Create Superuser**
   ```bash
   py manage.py createsuperuser
   ```

5. **Start Server**
   ```bash
   py manage.py runserver
   ```

6. **Access Application**
   - Home: `http://127.0.0.1:8000/`
   - All Tweets: `http://127.0.0.1:8000/tweets/`
   - Create Tweet: `http://127.0.0.1:8000/create/`

### Tweet App Features
- **Tweet Model Fields**:
  - Text content
  - Photo upload
  - User association
  - Timestamp

- **CRUD Operations**:
  - Create new tweets with text and images
  - View all tweets in card layout
  - Edit existing tweets (owner only)
  - Delete tweets (owner only)

- **UI Components**:
  - Gradient navbar with navigation
  - Card-based tweet display
  - Styled forms with validation
  - Responsive grid layout
  - Hover effects and animations

---

## 🎨 Design Features
- **Purple Gradient Background**: Modern diagonal gradient
- **Blue Gradient Navbar**: Professional navigation bar
- **White Content Cards**: Clean, rounded containers
- **Hover Effects**: Interactive elements with smooth transitions
- **Form Styling**: Custom input fields with focus states
- **Icon Integration**: Font Awesome icons throughout

---

## 🚀 Quick Start

```bash
cd project/tweet
py manage.py runserver
# Visit: http://127.0.0.1:8000/
```

---

## 📝 Notes

- Application uses SQLite for development
- Media files are stored in `media/` directory
- Bootstrap 5 and Font Awesome are loaded via CDN
- Admin panel integration for user management
- Responsive design works on mobile and desktop
- Custom CSS with gradient themes and animations

---

## 🛠️ Troubleshooting

### Common Issues

1. **Images not displaying**
   - Check `MEDIA_URL` and `MEDIA_ROOT` in settings
   - Ensure media URLs are configured in main `urls.py`
   - Verify image file formats (JPG, PNG recommended)

2. **Bootstrap/CSS not loading**
   - Check internet connection (CDN dependencies)
   - Verify Bootstrap and Font Awesome CDN links

3. **Database errors**
   ```bash
   py manage.py makemigrations
   py manage.py migrate
   ```

4. **Permission errors**
   - Ensure users can only edit/delete their own tweets
   - Check user authentication in views

---

## 📄 License

This project is for educational purposes. Feel free to use and modify as needed.

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

---

**Enjoy building with Django! 🎉**