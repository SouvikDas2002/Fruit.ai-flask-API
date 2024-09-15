# FAQ CRUD Application

This is a Flask-based CRUD (Create, Read, Update, Delete) application for managing FAQs, with data stored in MongoDB. The project allows users to perform operations on FAQ entries through various endpoints.

## Features

- **Create FAQ**: Add a new FAQ to the database.
- **Read FAQ**: Retrieve a specific FAQ or a list of all FAQs.
- **Update FAQ**: Modify an existing FAQ.
- **Delete FAQ**: Remove an FAQ by ID.

## Technologies Used

- **Flask**: Backend framework.
- **Flask-PyMongo**: For connecting to MongoDB.
- **MongoDB Atlas**: Cloud-based NoSQL database.
- **Flask-Cors**: To handle Cross-Origin Resource Sharing (CORS).
- **Waitress**: Production server for running the app.
- **Gunicorn**: Optional WSGI server.

## Project Setup

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. **Navigate to the backend directory**:

    ```bash
    cd fruit-ai-backend
    ```

3. **Create and activate a virtual environment**:

    ```bash
    python -m venv venv
    source venv/bin/activate  # For Windows: venv\Scripts\activate
    ```

4. **Install dependencies**:

    ```bash
    pip install -r requirements.txt
    ```

5. **Update the MongoDB URI** in `config.py`:

    ```python
    class Config:
        MONGO_URI = 'mongodb+srv://<username>:<password>@cluster0.mongodb.net/faqs?retryWrites=true&w=majority'
    ```

6. **Start the Flask server**:

    ```bash
    python app.py
    ```
7. **Run in Production using Waitress To serve the application in a production environment using Waitress, run:**:

    ```bash
    python run_server.py

    ```

8. Access the backend API at `http://localhost:5000`    or. The server will be hosted at http://0.0.0.0:8000.


## Endpoints

### 1. Create FAQ

- **URL**: `/faqs`
- **Method**: `POST`
- **Description**: Add a new FAQ to the database.

### 1. Get FAQ

- **URL**: `/faqs`
- **Method**: `GET`
- **Description**: Retrieve a list of all FAQs.

### 1. Get single FAQ

- **URL**: `/faqs/<faq_id>`
- **Method**: `GET`
- **Description**: Retrieve a specific FAQ by its ID.
- **URL Parameters**: faq_id (string): The ID of the FAQ to retrieve.

### 1. Update single FAQ

- **URL**: `/faqs/<faq_id>`
- **Method**: `PUT`
- **Description**: Update a specific FAQ by its ID.
- **URL Parameters**: faq_id (string): The ID of the FAQ to update.

### 1. Delete single FAQ

- **URL**: `/faqs/<faq_id>`
- **Method**: `DELETE`
- **Description**: Delete a specific FAQ by its ID.
- **URL Parameters**: faq_id (string): The ID of the FAQ to delete.

## Deployment

You can access the live application at the following URL:

- **Application URL**: [https://fruit-ai-flask-api-2.onrender.com](https://fruit-ai-flask-api-2.onrender.com)

## Contact

For any questions or support, feel free to contact me at [dev.souvik2002@gmail.com](mailto:dev.souvik2002@gmail.com).