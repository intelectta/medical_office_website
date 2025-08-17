# Mindful Wellness Psychology Office Website

A professional psychology office website built with Flask backend and React frontend, featuring internationalization support for English and Portuguese.

## Features

- **Professional Design**: Modern, calming design suitable for a psychology practice
- **Responsive Layout**: Works on desktop, tablet, and mobile devices
- **Internationalization**: Full support for English and Portuguese with language toggle
- **Contact Form**: Functional contact form with backend API integration
- **Services Display**: Dynamic services loaded from backend API
- **Interactive FAQ**: Accordion-style frequently asked questions
- **About Section**: Professional therapist biography and credentials

## Technology Stack

### Backend (Flask)
- Python Flask web framework
- SQLAlchemy for database management
- SQLite database
- Flask-CORS for cross-origin requests
- RESTful API endpoints

### Frontend (React + Vite)
- React 18 with modern hooks
- Vite for fast development and building
- Tailwind CSS for styling
- Shadcn/ui components
- Lucide React icons
- i18next for internationalization
- react-i18next for React integration
- Responsive design

## Internationalization

The website supports both English and Portuguese languages:
- **Language Toggle**: Located in the top-right corner of the homepage
- **Automatic Detection**: Detects user's browser language preference
- **Persistent Selection**: Language choice is saved in localStorage
- **Complete Translation**: All user-facing text is translated

### Supported Languages
- 🇺🇸 English (default)
- 🇧🇷 Portuguese (Português)

## API Endpoints

- `GET /api/services` - Retrieve all available services
- `POST /api/contact` - Submit contact form
- `GET /api/contact` - Retrieve contact submissions (admin)

## Setup Instructions

### Backend Setup
1. Navigate to the project directory
2. Create and activate virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Flask server:
   ```bash
   python src/main.py
   ```

### Frontend Development
The frontend is built and served from the Flask static directory. To modify the frontend:

1. Install Node.js dependencies (if making changes):
   ```bash
   cd frontend_src
   npm install
   ```
2. Make changes to frontend_src files
3. Build the frontend:
   ```bash
   npm run build
   ```
4. Copy built files to src/static/

### Adding New Languages
To add support for additional languages:

1. Update `frontend_src/i18n.js` with new language resources
2. Add the new language to the `LanguageToggle.jsx` component
3. Rebuild the frontend

## Deployment

The application is configured to run on any platform that supports Python Flask applications. The frontend is served as static files from the Flask application.

## Database

The application uses SQLite database with the following models:
- **User**: Basic user management
- **Contact**: Contact form submissions

## Security Features

- CORS configured for cross-origin requests
- Input validation on contact forms
- SQL injection protection via SQLAlchemy ORM

## Customization

To customize the website with your own data:
1. Update the translation files in `frontend_src/i18n.js`
2. Modify the services data in the Flask backend
3. Replace placeholder images in the assets folder
4. Update contact information and credentials

## License

This project is created for educational and professional use.

## Contact

For questions about this website, please use the contact form on the website or reach out directly.

