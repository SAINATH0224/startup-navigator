# 🚀 Startup Navigator – Comprehensive Guide to Startups

> A modern, responsive, AI-powered web application helping aspiring entrepreneurs learn everything about building a startup in India.

---

## 🌟 Live Demo

Open `index.html` in any modern web browser — no server required!

---

## ✨ Features

| Feature | Description |
|---|---|
| 📚 **10 Topic Guides** | In-depth step-by-step articles on Registration, Funding, Legal, Hiring, Marketing, Taxation & more |
| 🤖 **AI Search** | Smart keyword-matching assistant that answers startup questions using stored articles |
| 📎 **20+ Resources** | Government portals, templates, legal docs, funding links, and tools |
| 🔐 **User Auth** | Register, Login, Logout with session management |
| ⚙️ **Admin Dashboard** | Full CRUD for articles and resources, platform statistics |
| 📱 **Responsive** | Works perfectly on desktop, tablet, and mobile |
| 🌙 **Dark Mode** | Premium dark UI with glassmorphism and smooth animations |
| 💾 **Offline Ready** | All data stored in localStorage — works without internet |

---

## 🎯 Demo Credentials

### Admin Account
- **Email:** `admin@startupnav.com`
- **Password:** `Admin@123`

### Test User
- Register a new account on the Login page with any email/password

---

## 📁 Folder Structure

```
Freelance_app/
├── index.html              ← Home page
├── explore.html            ← Explore Topics
├── topic-detail.html       ← Individual Topic View
├── ai-search.html          ← AI Search Chat
├── resources.html          ← Resources Hub
├── about.html              ← About Page
├── contact.html            ← Contact Form
├── login.html              ← Login / Register
├── admin.html              ← Admin Dashboard
├── css/
│   ├── main.css            ← Design tokens, typography, navbar, footer
│   ├── components.css      ← Cards, buttons, forms, modals, tables
│   └── pages.css           ← Page-specific styles
└── js/
    ├── data.js             ← Seed data (10 topics, 20+ resources)
    ├── storage.js          ← LocalStorage CRUD helpers
    ├── auth.js             ← Authentication module
    ├── ai.js               ← AI keyword-matching engine
    ├── app.js              ← Shared utilities (navbar, toast, helpers)
    └── admin.js            ← Admin dashboard operations
```

---

## 🤖 AI Integration

The AI search engine uses a **multi-layer keyword matching** approach:

1. **Curated FAQ Layer** — 10 hand-crafted Q&A pairs for common questions (registration, funding, taxes, etc.)
2. **Article Search Layer** — Tokenizes the query and scores all stored articles by title match, keyword match, and content match
3. **Fallback Layer** — Generic helpful response listing available topics

All responses are formatted in Markdown and rendered as styled HTML in the chat interface.

**AI doesn't require an API key** — it works entirely offline using the stored knowledge base.

---

## 🏗️ Architecture

```
User → Web Application (HTML/CSS/JS)
              ↓
       localStorage (Database)
       ├── Topics/Articles
       ├── Resources
       ├── Users & Sessions
       └── Search History
              ↓
       AI Engine (js/ai.js)
       ├── FAQ matching
       ├── Relevance scoring
       └── Response formatting
              ↓
       Formatted Response → Chat UI
```

---

## 🚀 How to Run

### Option 1: Direct Browser (Simplest)
1. Download or clone this repository
2. Double-click `index.html` to open in your browser
3. That's it! No build step, no server required.

### Option 2: Local Server (Recommended for best experience)
```bash
# Using Python
python -m http.server 3000

# Using Node.js
npx serve .

# Using VS Code
Install "Live Server" extension → Right-click index.html → Open with Live Server
```

Then open `http://localhost:3000`

---

## 🌐 Deployment

### GitHub Pages (Free)
1. Push the project to a GitHub repository
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your site is live at `https://yourusername.github.io/repo-name/`

### Netlify (Free + Custom Domain)
1. Go to [netlify.com](https://netlify.com)
2. Drag & drop the project folder to the deploy area
3. Instant live URL!

### Vercel (Free)
1. Go to [vercel.com](https://vercel.com)
2. Import your GitHub repository
3. Deploy with one click

---

## 📋 Topics Covered

1. 🏢 **Company Registration** — SPICe+, DIN, DSC, Certificate of Incorporation
2. 💰 **Funding** — Bootstrapping, Angels, Seed, VC, Government grants
3. ⚖️ **Legal Compliance** — IP, Contracts, Privacy Policy, Labour Law
4. 👥 **Hiring** — Job posts, interview process, ESOPs, onboarding
5. 🎨 **Branding** — Name, logo, colors, brand voice, style guide
6. 📣 **Marketing** — SEO, content, social, email, paid ads, growth hacking
7. 🧾 **Taxation** — GST, TDS, Advance Tax, Section 80-IAC, Angel Tax
8. 📊 **Fundraising** — Pitch deck, term sheet, due diligence, cap table
9. 📈 **Business Growth** — PMF, North Star Metric, unit economics, scaling
10. 🤖 **AI Tools** — GitHub Copilot, ChatGPT, AI for support/sales/legal

---

## 🛠️ Tech Stack

- **HTML5** — Semantic markup
- **CSS3** — Custom properties, glassmorphism, animations
- **Vanilla JavaScript** — No frameworks, no dependencies
- **Google Fonts** — Inter + Space Grotesk
- **LocalStorage** — Client-side database
- **No build step** — Works directly in browser

---

## 🔐 Security Notes

This is a **demo application**. The auth system uses `btoa()` encoding (not real encryption). For production:
- Replace with a proper backend (Firebase, Supabase, etc.)
- Use bcrypt or Argon2 for password hashing
- Implement HTTPS
- Add CSRF protection
- Use proper session tokens (JWT)

---

## 📝 License

MIT License — Free to use, modify, and distribute.

---

Made with ❤️ for the Indian startup community. 🇮🇳
