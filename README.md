# 🌐 Multi-Cloud Interoperability Demo (AWS + GCP)

This project demonstrates how to build and deploy a web application using a **multi-cloud architecture**. The frontend is hosted on **Amazon S3 (AWS)**, while the backend is deployed using **Cloud Run (GCP)**. It showcases seamless cross-platform communication between services from different cloud providers.

---

## 🚀 Architecture Overview

- **Frontend**: Static website (HTML/CSS/JS) hosted on **AWS S3**
- **Backend**: Python API deployed on **GCP Cloud Run**
- **Interoperability**: JavaScript `fetch()` calls the GCP endpoint from AWS-hosted frontend

```
User → AWS S3 (Static Website)
     → GCP Cloud Run (API Request)
     ← Response from GCP
```

---

## 🧱 Technologies Used

- **AWS S3** (Static website hosting)
- **GCP Cloud Run** (Python backend)
- **Functions Framework** for GCP
- **HTML/CSS/JavaScript** frontend
- **CORS** for cross-cloud request handling

---

## 📂 Project Structure

```
/frontend
  └── index.html        # Static webpage

/backend
  ├── main.py           # GCP backend function
  └── requirements.txt  # Python dependencies
```

---

## ⚙️ How to Run

### Frontend (on AWS S3)
1. Upload `index.html` to a new S3 bucket
2. Enable static website hosting
3. Make bucket objects public or use CloudFront (optional)

### Backend (on GCP Cloud Run)
1. Deploy `main.py` using Cloud Run with `functions-framework`
2. Ensure CORS headers are included
3. Replace the API URL in `index.html` with your deployed endpoint

---

## 📬 API Response Example

```json
"Hello from GCP backend!"
```

---

