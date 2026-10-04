# Flask Chatbot Agent

A Python-based chatbot agent built with Flask. Simple, lightweight, and easy to extend. Chat with an AI agent through your web browser.

## 📸 Screenshot

![Flask Chatbot Agent Repository](./flask-chatbot-agent.png)

**View the chat interface:** Open `http://localhost:5000` in your web browser after running the app.

## Features

- **Flask-based web server**: Lightweight and easy to deploy
- **HTML chat interface**: Clean, responsive design with message bubbles
- **Static file serving**: Serves CSS and JavaScript from the `static/` directory
- **Easy to extend**: Add new responses and routes simply
- **Template-based**: Uses Jinja2 HTML templates for dynamic content

## 🚀 Quick Start

```bash
# 1. Install dependencies
pip install flask

# 2. Run the application
python app.py

# 3. Open in browser
# Visit: http://localhost:5000
# The chat will be available at the root URL
```

## 🛠️ Project Structure

```
agent/
├── app.py              # Flask application factory and routing
├── templates/
│   ├── index.html      # Home page with chat interface
│   └── chat.html       # Chat message rendering and logic
└── static/
    ├── style.css       # Responsive styling with message animations
    └── script.js       # Client-side chat logic and fetch API
```

## 💡 How It Works

1. **Server-side** (`app.py`): Flask handles HTTP requests, renders templates, and serves static files
2. **Client-side** (`static/script.js`): Fetches data asynchronously, handles user input, displays responses
3. **Templates** (`templates/`): Jinja2 HTML with dynamic content insertion

You can extend the chatbot by:
- Adding new response functions in `app.py`
- Modifying the chat logic in `static/script.js`
- Updating the styles in `static/style.css`
- Adding new HTML templates in `templates/`

## 📦 Deployment

```bash
# Production deployment
gunicorn app.py

# Or use Flask's built-in server
flask run

# Docker (optional)
# docker build -t flask-chatbot .
```

## 📜 License

MIT

---

**K.bhalavardt, MIT Student**