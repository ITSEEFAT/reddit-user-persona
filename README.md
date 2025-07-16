
# 🔍 Reddit User Persona Generator using Gemini AI

A Python-powered tool that scrapes Reddit user activity (posts + comments) and generates a detailed **user persona** using **Google Gemini 1.5 Flash**.

It’s designed for digital behavior analysts, researchers, or AI hobbyists looking to understand a Reddit user's personality traits, goals, and interests based on their activity.

---

## 🚀 Features

- ✅ Fetches recent **Reddit posts (20)** and **comments (50)** of any user
- 🤖 Uses **Gemini AI (Google Generative AI)** to analyze and summarize user behavior
- 📁 Saves:
  - Raw user data
  - AI-generated user persona with citations and quotes

---

## 📸 Sample Output

Generated persona includes:

```
Name: TechExplorer
Age Group: 25-34
Occupation: Software Developer
Personality Traits: Curious, Analytical, Helpful
Goals: Stay updated with tech trends, contribute to discussions
Pain Points: Dislikes vague questions or low-effort content
...
```

---

## 🛠️ Setup Instructions

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/yourusername/reddit-user-persona.git
cd reddit-user-persona
```

---

### 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

---

### 3️⃣ Add Your API Keys

Create a `.env` file in the root directory:

```env
GEMINI_API_KEY=your_gemini_api_key
REDDIT_CLIENT_ID=your_reddit_client_id
REDDIT_CLIENT_SECRET=your_reddit_client_secret
REDDIT_USER_AGENT=reddit-user-persona by /u/yourusername
```

---

### 4️⃣ Run the Script

```bash
python main.py
```

🔗 When prompted, enter a Reddit profile URL, e.g.:

```
https://www.reddit.com/user/spez/
```

---

## 📂 Output Files

All files are saved inside an `outputs/` folder:

| File                     | Description                          |
|--------------------------|--------------------------------------|
| `username_raw.txt`       | Raw Reddit data (posts + comments)   |
| `username_persona.txt`   | AI-generated persona with quotes     |

---

## 🧠 How It Works

This project uses:

- **PRAW** – Python Reddit API Wrapper to fetch user content
- **Google Generative AI SDK** – To analyze content and generate personas
- **Gemini 1.5 Flash** – Fast, cost-efficient model for persona generation

Prompt includes structure like:
- Name, Age Group
- Interests & Subreddits
- Sample Quotes
- Personality + Citations

---

## 📌 Notes

- Do **not** commit your `.env` file.
- Reddit users with no public posts/comments will return blank files.
- Gemini API key must be enabled from [Google AI Studio](https://makersuite.google.com/app/apikey)

---

## 💡 Future Improvements

- Web-based UI using Streamlit
- Batch process multiple users
- Export to PDF or HTML

---

## 🧑‍💻 Author

**Seefat**, for a GitHub-based ML assignment  
Connect on [GitHub](https://github.com/yourusername)

---

## 📄 License

MIT License. Use freely, but credit appreciated!
"# reddit-user-persona" 
