# 💰 Family Finance — AI-Powered Expense Tracker

A free, private, mobile-first Progressive Web App (PWA) for tracking family expenses using natural chat messages. Powered by Google Gemini AI. No server, no subscription, no account required.

---

## ✨ Features

- **Natural language input** — type like you talk: *"spent 3500 on groceries"* or *"paid electricity bill 4200"*
- **AI-powered parsing** — Gemini AI understands and categorizes every message automatically
- **Budget tracking** — set monthly limits per category with visual progress bars
- **Dashboard** — live balance, monthly income vs spending, category breakdown
- **Full history** — every transaction with date, category, and delete option
- **100% private** — all data stored on your device, never sent to any server
- **Works offline** — loads from cache after first visit
- **Installable** — appears as a real app icon on Android home screen

---

## 📱 How to Install on Android (Free)

> No app store needed. Install directly from the browser in 2 minutes.

**Step 1 — Deploy the app** *(see Deployment section below)*

**Step 2 — Install on Android**
1. Open **Chrome** on your Android phone
2. Navigate to your app URL (e.g. `https://yourusername.github.io/family-finance`)
3. Tap the **3-dot menu** (⋮) in the top right
4. Tap **"Add to Home screen"**
5. Tap **Add** — the app icon appears on your home screen ✅

**Step 3 — Share with family**
- Send the same URL to every family member
- Each person installs it the same way
- Everyone shares the same data automatically (stored in shared localStorage)

---

## 🚀 Deployment — Completely Free

### Option A: GitHub Pages *(Recommended)*

1. Create a free account at [github.com](https://github.com)
2. Click **New repository** → name it `family-finance` → set to **Public** → Create
3. Click **Add file** → **Upload files** → upload `family-finance-pwa.html`
4. After upload, click the file → click the pencil ✏️ icon → rename it to `index.html` → Commit
5. Go to **Settings** → **Pages** → under Source, select **main** branch → click **Save**
6. Wait ~2 minutes → your app is live at:
   ```
   https://yourusername.github.io/family-finance
   ```

## 🤖 AI Setup — Free Gemini API Key

The app uses **Google Gemini 2.0 Flash** — free tier gives **1,500 messages/day** (a typical family uses ~10–20/day).

**Get your free API key:**

1. Go to [aistudio.google.com](https://aistudio.google.com)
2. Sign in with any Google account
3. Click **"Get API key"** → **Create API key** → Copy it
4. Open the app → paste the key when prompted → tap **Start Tracking**

> Your API key is stored only on your device (localStorage). It is never sent to any third party.

---

## 💬 How to Use — Chat Commands

The AI understands natural language. Here are examples:

### Recording Expenses
```
spent 2500 on groceries
paid school fees 15000
electricity bill 4200
bought medicine 800
transport 350 today
```

### Recording Income
```
received salary 95000
got freelance payment 25000
wife salary 80000 received
```

### Setting Budgets
```
set food budget to 20000
transport budget 8000
groceries limit 15000 per month
```

### Queries
```
what is my balance?
show this month summary
what did I spend most on?
how much left in food budget?
undo last entry
```

---

## 📂 Project Structure

```
index.html          ← entire app (single file, no dependencies)
README.md           ← this file
```

The app is intentionally a single HTML file with no build step, no npm, no framework dependency. Just host the file and it works.

---

## 🗂️ Expense Categories

| Category | Icon | Use for |
|---|---|---|
| Food & Dining | 🍽️ | Restaurants, takeaway, cafes |
| Groceries | 🛒 | Supermarket, vegetable market |
| Transport | 🚗 | Fuel, bus, three-wheeler, Uber |
| Utilities | 💡 | Electricity, water, internet, phone |
| Health | 💊 | Medicine, doctor, hospital |
| Education | 📚 | School fees, books, tuition |
| Entertainment | 🎬 | Outings, subscriptions, events |
| Clothing | 👕 | Clothes, shoes, accessories |
| Salary | 💼 | Monthly salary (income) |
| Freelance | 💻 | Freelance / side income |
| Other | 📦 | Anything else |

---

## 🔒 Privacy & Data

| What | Where stored | Who can see it |
|---|---|---|
| Transactions | Device (localStorage) | Only people using this device/browser |
| Budgets | Device (localStorage) | Only people using this device/browser |
| Gemini API key | Device (localStorage) | Only you |
| Your messages | Sent to Google Gemini API | Google processes them to parse intent (no personal data stored per Google's free API terms) |

**No account, no login, no cloud sync.** Data lives in the browser on the device.

---

## 🛠️ Tech Stack

| Layer | Technology | Cost |
|---|---|---|
| Frontend | Pure HTML + CSS + JavaScript | Free |
| AI | Google Gemini 2.0 Flash API | Free (1,500 req/day) |
| Storage | Browser localStorage | Free |
| Hosting | GitHub Pages / Vercel / Netlify | Free |
| PWA | Service Worker + Web App Manifest | Built-in |
| Fonts | Google Fonts (DM Sans, DM Mono) | Free |

**Total monthly cost: Rs 0**

---

## 🔧 Customisation

### Change Currency
Search for `Rs` in `index.html` and replace with your currency symbol (e.g. `LKR`, `$`, `€`).

### Change App Name
Replace `Family Finance` in the `<title>` tag and in the manifest `name` field near the bottom of the file.

### Change Language / Tone
In the `systemPrompt` variable inside the `sendMsg()` function, edit the first line to change how the AI responds (e.g. change "Sri Lankan family" to match your region).

---

## ❓ Troubleshooting

**"Add to Home screen" option not showing?**
Make sure you are using Chrome browser, not Samsung Internet or another browser.

**AI not responding?**
Check that your Gemini API key is correct. Go to Budget → Settings → Change API key.

**Data disappeared?**
Data is stored in the browser. Clearing browser data / cache will erase it. Avoid clearing site data for this app.

**App not loading offline?**
Visit the app online once first. The service worker will cache it for offline use after the first visit.

---

## 📄 License

Free to use for personal and family use. Built with ❤️ for families who want to track expenses without paying for apps or subscriptions.
