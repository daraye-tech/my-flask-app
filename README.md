# 🐍 My Flask App with Docker

This is a simple Flask web application that exposes a JSON API endpoint at `/hello`. The project includes a `Dockerfile` for containerization and is ready for deployment or local development.

---

## 🚀 Features

- ✅ Lightweight Flask API
- 🐳 Dockerized for easy portability
- 🔥 Ready to run in any environment (local, cloud, CI/CD)
- 📦 Clean and minimal dependencies

---

## 📁 Project Structure

my-flask-app/
├── app.py # Main Flask app
├── requirements.txt # Python dependencies
├── Dockerfile # Container instructions
└── README.md # Project documentation

yaml
Copy
Edit

---

## 🔧 Requirements

- Python 3.11+
- Docker installed (for container usage)
- Git (if cloning)

---

## ▶️ How to Run Locally (Without Docker)

```bash
# 1. Clone the repository
git clone https://github.com/daraye-tech/my-flask-app.git
cd my-flask-app

# 2. Create a virtual environment
python3 -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Run the app
python app.py
The API will be available at:
👉 http://localhost:5000/hello

🐳 How to Run with Docker
1. Build the Docker image
bash
Copy
Edit
docker build -t my-flask-app .
2. Run the container
bash
Copy
Edit
docker run -p 5000:5000 my-flask-app
Now you can access the endpoint via:
👉 http://localhost:5000/hello

🔥 Example API Response
json
Copy
Edit
{
  "message": "Hello, world!"
}
⚙️ requirements.txt
Only includes necessary dependencies:

nginx
Copy
Edit
flask
