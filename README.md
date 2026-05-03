# 🚀 Gemma E4B UI

A React-based frontend for interacting with the Gemma LLM via a FastAPI backend.
Supports text chat and image uploads in a simple, responsive interface.

---

## ✨ Features

* 💬 Chat interface (`/chat`)
* 🖼️ Image upload support (`/chat-file`)
* ✍️ Markdown-rendered responses
* 📱 Responsive UI
* ⚡ Fast and minimal design

---

## 📦 Requirements

* Node.js 18+
* npm

---

## ⚙️ Setup Instructions

### 1. Clone the repository

```bash id="x1q7sm"
git clone https://github.com/sathvik1607/Gemma_E4B_UI.git
cd Gemma_E4B_UI
```

---

### 2. Install dependencies

```bash id="n2k9pl"
npm install
```

---

## 🔑 Environment Configuration

Create a `.env` file in the root directory:

```env id="c7m4zd"
VITE_API_BASE_URL=http://localhost:8000
```

⚠️ Make sure this matches your backend URL.

---

## ▶️ Run the App

```bash id="r8j2vd"
npm run dev
```

App runs at:

```
http://localhost:5173
```

---

## 📡 API Integration

### 1. Text Chat

**POST** `/chat`

```json id="p3f8lw"
{
  "message": "Hello"
}
```

---

### 2. Image + Text

**POST** `/chat-file`

Form data:

* `file`: image
* `mssg`: text

---

## 🧠 Notes

* Image uploads are supported (max 5MB)
* Ensure backend is running before using the app
* API base URL must be set correctly in `.env`

---

## 📄 License

MIT
