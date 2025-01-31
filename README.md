# FAQ Management System

## Installation

### 1. Clone the repository:
```bash
git clone https://github.com/your-username/your-repo-name.git
```

### 2. Navigate to the project directory:
```bash
cd your-repo-name
```

### 3. Install dependencies:
```bash
pip install -r requirements.txt
```

### 4. Run migrations:
```bash
python manage.py migrate
```

### 5. Start the server:
```bash
python manage.py runserver
```

## API Usage

### Fetch FAQs in English (Default):
```http
GET /api/faqs/
```

### Fetch FAQs in Hindi:
```http
GET /api/faqs/?lang=hi
```

### Fetch FAQs in Bengali:
```http
GET /api/faqs/?lang=bn
```

## Running with Docker

### Build and start the containers:
```bash
docker-compose up
```

### Access the API at:
```
http://localhost:8000/api/faqs/
```

## Contribution Guidelines

### 1. Fork the repository.

### 2. Create a new branch for your feature:
```bash
git checkout -b feature-name
```

### 3. Commit your changes:
```bash
git commit -m "feat: Add feature-name"
```

### 4. Push to the branch:
```bash
git push origin feature-name
```

### 5. Open a pull request.

## Features Implemented
- **FAQ Model:** Supports multilingual translations for questions and answers.
- **WYSIWYG Editor:** Integrated `django-ckeditor` for rich text formatting.
- **REST API:** Supports language selection via query parameters.
- **Caching:** Uses Redis to cache translations for improved performance.
- **Automated Translations:** Uses `googletrans` to automatically translate questions during creation.
- **Admin Panel:** User-friendly interface for managing FAQs.
- **Unit Tests:** Includes unit tests for models and API endpoints.

## Technology Stack
- **Backend Framework:** Django (Python)
- **WYSIWYG Editor:** `django-ckeditor`
- **Translation:** `googletrans`
- **Caching:** Redis
- **Testing:** `pytest`
- **Linting:** `flake8` (PEP8 compliance)
- **Version Control:** Git

## Example API Requests

### Fetch FAQs in English (Default):
```bash
curl http://localhost:8000/api/faqs/
```

### Fetch FAQs in Hindi:
```bash
curl http://localhost:8000/api/faqs/?lang=hi
```

### Fetch FAQs in Bengali:
```bash
curl http://localhost:8000/api/faqs/?lang=bn
```

## License
This project is licensed under the MIT License. See the LICENSE file for details.

## How to Use
1. Replace `your-username` and `your-repo-name` with your actual GitHub username and repository name.
2. Save this content in a file named `README.md` in the root directory of your project.
3. Push the changes to GitHub:
```bash
git add README.md
git commit -m "docs: Add detailed README file"
git push origin main
