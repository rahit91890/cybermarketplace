# Cybermarketplace

## Project Description

Cybermarketplace is a modern e-commerce platform designed to provide a secure and scalable marketplace solution. Built with cutting-edge technologies, this platform enables seamless buying and selling experiences with robust backend infrastructure and an intuitive frontend interface.

## Tech Stack

### Backend
- **Python**: Core backend development language
- **Django**: High-level Python web framework for rapid development
- **Django REST Framework**: Building powerful and flexible APIs

### Frontend
- **React/Modern JavaScript**: Interactive user interface
- **Responsive Design**: Mobile-first approach

### DevOps & Deployment
- **Docker**: Containerization for consistent development and deployment
- **Docker Compose**: Multi-container orchestration

## Prerequisites

Before you begin, ensure you have the following installed:
- Python 3.8 or higher
- Docker Desktop (or Docker Engine + Docker Compose)
- Git

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/rahit91890/cybermarketplace.git
cd cybermarketplace
```

### 2. Environment Configuration
Copy the example environment file and configure your settings:
```bash
cp .env.example .env
```

Edit the `.env` file with your specific configuration values (database credentials, API keys, etc.).

### 3. Using Docker (Recommended)

Build and start all services using Docker Compose:
```bash
docker-compose up --build
```

The application will be available at:
- Frontend: `http://localhost:3000`
- Backend API: `http://localhost:8000`

### 4. Manual Setup (Without Docker)

#### Backend Setup
```bash
cd backend
pip install -r requirements.txt
python manage.py migrate
python manage.py createsuperuser
python manage.py runserver
```

#### Frontend Setup
```bash
cd frontend
npm install
npm start
```

## Usage Guide

### Running the Application

**With Docker:**
```bash
# Start services
docker-compose up

# Stop services
docker-compose down

# View logs
docker-compose logs -f
```

**Without Docker:**
```bash
# Backend (in one terminal)
cd backend
python manage.py runserver

# Frontend (in another terminal)
cd frontend
npm start
```

### Accessing the Admin Panel
1. Navigate to `http://localhost:8000/admin`
2. Log in with the superuser credentials created during setup
3. Manage products, users, and orders from the admin interface

### API Documentation
Once the backend is running, API documentation is available at:
- `http://localhost:8000/api/docs/`

## Project Structure
```
cybermarketplace/
├── backend/           # Django backend application
├── frontend/          # React frontend application
├── docker-compose.yml # Docker orchestration file
├── .env.example       # Environment variables template
├── .gitignore         # Git ignore rules
└── README.md          # Project documentation
```

## Contributing

We welcome contributions! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact Information

**Codaphics**

For inquiries, support, or collaboration opportunities, please reach out:

- **Website**: [codaphics.com](https://codaphics.com)
- **Email**: contact@codaphics.com
- **Project Repository**: [github.com/rahit91890/cybermarketplace](https://github.com/rahit91890/cybermarketplace)

---

*Built with ❤️ by Codaphics*
