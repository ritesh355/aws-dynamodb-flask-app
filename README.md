# aws-dynamodb-flask-app

A simple **Flask + AWS DynamoDB CRUD application** to manage tasks with a clean UI using Bootstrap. This app allows you to **Add, Edit, and Delete tasks** stored in a DynamoDB table.

---

![](images/project.png)

---
## Project Structure

```
aws-dynamodb-flask-app/
│
├── app.py                     # Main Flask application
├── requirements.txt           # Python dependencies
├── README.md                  # Project description / instructions
│
├── templates/                 # HTML templates
│   └── index.html             # Single-page template with Add/Edit/Delete modals
│
├── static/                    # Static files (CSS, JS, images)
│   ├── style.css              # Custom CSS for styling, colors, etc.
│   └── images/                # Optional images/icons
│
├── venv/                      # Python virtual environment (ignored in git)
│
└── .gitignore                 # Ignore venv, __pycache__, etc.
```

---

## Features

* **Single-page CRUD interface** using Bootstrap modals
* **DynamoDB integration** for storing tasks
* **Add task** with unique Task ID, title, and status
* **Edit task** directly from modal
* **Delete task** with confirmation
* **Responsive design** with modern styling

---

## Setup Instructions

1. **Clone the repository**:

```bash
git clone 
cd aws-dynamodb-flask-app
```

2. **Create a virtual environment**:

```bash
python3 -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. **Install dependencies**:

```bash
pip install -r requirements.txt
```

4. **Configure AWS credentials** (for DynamoDB access):

```bash
aws configure
```

5. **Run the Flask app**:

```bash
python app.py
```

6. **Open in browser**:

```
http://127.0.0.1:5000/
```

---

## DynamoDB Table Structure

* **Table Name:** `Users`
* **Primary Key:** `TaskID` (String)
* **Attributes:** `Title` (String), `Status` (String)

---

## Notes

* All modals for Add/Edit/Delete are handled in **index.html** for simplicity.
* Custom styles are in **static/style.css**.
* This project is intended for **local development**. Docker setup and CI/CD can be added later if needed.

---


---

## Author

Ritesh Singh

---

