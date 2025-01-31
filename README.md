# FAQ Management System

## Installation
1. Clone the repository.
2. Install dependencies: `pip install -r requirements.txt`.
3. Run migrations: `python manage.py migrate`.
4. Start the server: `python manage.py runserver`.

## API Usage
- Fetch FAQs in English: `GET /api/faqs/`
- Fetch FAQs in Hindi: `GET /api/faqs/?lang=hi`
- Fetch FAQs in Bengali: `GET /api/faqs/?lang=bn`

## Running with Docker
1. Build and start the containers: `docker-compose up`.
2. Access the API at `http://localhost:8000/api/faqs/`.