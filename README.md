# 🧪 Flask API Sandbox  

A lightweight sandbox project for learning how to build simple **RESTful APIs** using **Flask**.  
It’s your playground to explore backend development fundamentals in Python 🚀  

---

## 📘 About The Project  

This project was built as a **hands-on learning exercise** to understand how APIs work under the hood.  
The goal was to create a minimal yet functional backend capable of handling basic HTTP requests and returning JSON responses.  

### 🔍 What You’ll Learn  
- 🧭 Basic routing in Flask  
- ⚙️ Handling **GET** and **POST** requests  
- 💬 Sending & receiving **JSON** payloads  
- 🛠️ Setting up a local development environment  

---

## ⚙️ Getting Started  

Follow these steps to get your local environment up and running 👇  

### 🧩 Prerequisites  
Make sure you have the following installed:  
- 🐍 Python 3.x  
- 📦 pip  

---

### 💻 Installation  

1. **Clone the repository**  
   ```bash
   git clone https://github.com/your-username/your-repository-name.git
   ```

2. **Navigate to the project directory**  
   ```bash
   cd your-repository-name
   ```

3. **Create and activate a virtual environment**  

   - **On macOS/Linux:**  
     ```bash
     python3 -m venv venv
     source venv/bin/activate
     ```

   - **On Windows:**  
     ```bash
     python -m venv venv
     .\venv\Scripts\activate
     ```

4. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```
   > 💡 To create `requirements.txt`, run:  
   > `pip freeze > requirements.txt` after installing Flask.  

---

## 🚀 Running the Application  

Start the Flask development server:  
```bash
flask run
```

The API will be live at 👉 **http://127.0.0.1:5000**

---

## 🔗 Usage  

You can test endpoints using tools like **curl** or **Postman**.

---

### 🟢 GET `/api/hello`  

**Returns** a simple welcome message.

#### ✅ Request:
```bash
curl http://127.0.0.1:5000/api/hello
```

#### 💬 Response:
```json
{
  "message": "Hello! This is my first Flask API."
}
```

---

### 🟣 POST `/api/echo`  

**Echoes back** the JSON data sent in the request body.

#### ✅ Request:
```bash
curl -X POST   -H "Content-Type: application/json"   -d '{"name": "User", "data": "Some sample data"}'   http://127.0.0.1:5000/api/echo
```

#### 💬 Response:
```json
{
  "received_data": {
    "name": "User",
    "data": "Some sample data"
  },
  "status": "success"
}
```

---

## 🧰 Built With  
- 🐍 [Python](https://www.python.org/)  
- 🔥 [Flask](https://flask.palletsprojects.com/)  

---

## 📜 License  
Distributed under the **MIT License**.  
See the `LICENSE` file for more information.  
