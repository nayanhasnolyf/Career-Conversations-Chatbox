# Career Conversations Chatbox

**Career Conversations Chatbox** is a personal AI assistant that lives on your website and answers questions about your professional profile, experience, and skills. It uses OpenAI's Gemini model, Pushover for real-time notifications, and Gradio for a simple chat interface.

---

## ✨ Features

- Uses OpenAI-compatible Gemini API for intelligent responses.
- Loads your LinkedIn profile and career summary from PDF and text files.
- Sends push notifications via Pushover when a user provides contact details or asks an unknown question.
- Handles OpenAI function/tool calls dynamically.
- Provides a simple chat interface with Gradio.
- Easily customizable system prompt to match your personal branding.

---

## 📂 Project Structure
```bash
me/
 ├── profile.pdf
 ├── summary.txt
.env
main.py
requirements.txt
```
---


---

## ⚙️ Setup

1. **Clone the repository**

   ```bash
   git clone https://github.com/yourusername/career-conversations-chatbox.git
   cd career-conversations-chatbox

   ```
2. **Install Dependencies**

   ```bash
   pip install -r requirements.txt
   ```
3. **Create a .env file**

   ```bash
     PUSHOVER_TOKEN=your_pushover_app_token
    PUSHOVER_USER=your_pushover_user_key
    GEMINI_API_KEY=your_gemini_api_key
    ```
4. **Add your files**

    Place your profile.pdf and summary.txt inside a me/ folder.

5. **Run the app**
    ```bash
   python main.py
   ```

---
**🚀 How it Works**

Users chat with the assistant through a Gradio web interface.

If the assistant cannot answer a question, it records it using record_unknown_question and sends you a push notification.

If the user shares their email, it records their details using record_user_details and notifies you.

The assistant stays in character, representing you professionally.

---

**🔒 Notes**

Never commit your .env file — keep your keys private!

Make sure your profile.pdf and summary.txt are updated regularly.

Adapt the system prompt in main.py to reflect your style and tone.

---

**📌 To-Do Ideas**

Add async support for push notifications.

Improve PDF parsing and formatting.

Deploy to Fly.io, Heroku, or Render for easy public access.

Style the Gradio interface for a more personal look.

---

**📜 License**

This project is open source — feel free to adapt it for your own personal career chatbox.

---
## This Project is made by Nayan.
---
