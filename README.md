# 💰 Family Finance App — User Manual

Your personal family expense tracker. Chat naturally to record expenses, check your balance, and stay on budget. Works on phone and laptop. All free.

---

## 📱 Installing on Your Phone (Android)

1. Open **Chrome** on your Android phone
2. Go to your app link (the GitHub Pages URL)
3. Tap the **3-dot menu ⋮** at the top right
4. Tap **"Add to Home screen"**
5. Tap **Add**

The app now appears on your home screen like a normal app. Tap it to open anytime — no app store needed.

---

## 🤖 Setting Up the AI (First Time Only)

The AI understands what you type and records it automatically. You need a free API key to activate it.

**Get your free key:**
1. Go to **console.groq.com**
2. Sign up with your email (free, no credit card)
3. Click **API Keys** in the left menu
4. Click **Create API key** → give it any name → click **Submit**
5. Copy the key shown (starts with `gsk_...`) — you won't see it again

**Enter the key in the app:**
1. Open the app → tap the **Budget** tab at the bottom
2. Scroll down to **Groq AI key**
3. Paste your key → tap **Save**
4. Tap **🔌 Test connection** — it should say "Connected!"

---

## ☁️ Setting Up Sync (Phone + Laptop)

This lets your phone and laptop show the same data. Do this once.

**Step 1 — Create a free Firebase database**
1. Go to **console.firebase.google.com** and sign in with Google
2. Click **Add project** → type any name → click **Continue** twice
3. In the left sidebar, click **Build** → **Realtime Database**
4. Click **Create database**
5. Select **asia-southeast1 (Singapore)** from the dropdown → click **Next**
6. Select **Start in test mode** → click **Enable**
7. You will now see a URL at the top of the page like this:
   ```
   https://your-project-default-rtdb.asia-southeast1.firebasedatabase.app
   ```
8. **Copy that URL**

**Step 2 — Paste the URL in the app (do this on BOTH devices)**
1. Open the app → tap **Budget** tab → scroll to **☁️ Family sync**
2. Paste the URL into the field
3. Tap **Enable Sync →**
4. It will say "✓ Sync enabled"

Repeat on your other device with the same URL. Both devices will now stay in sync automatically.

---

## 💬 How to Use the Chat

Just type naturally — the AI figures out the rest.

**Recording an expense**
```
spent 2500 on groceries
paid electricity bill 4200
bought medicine 800
kids school fees 15000
transport 350
```

**Recording income**
```
received salary 95000
wife salary 80000
got freelance payment 25000
```

**Setting a budget limit**
```
set food budget 20000
transport budget 8000
groceries limit 15000
```

**Checking your money**
```
what is my balance?
show this month summary
what did I spend most on?
how much left in food budget?
```

**Made a mistake?**
```
undo
undo last entry
```

---

## 📊 The Four Tabs

| Tab | What it shows |
|---|---|
| 💬 Chat | Type here to record expenses and ask questions |
| 📊 Dashboard | Your balance, spending by category, budget progress |
| 📋 History | Every transaction this month with delete button |
| 🎯 Budget | Set monthly limits, manage sync, change API key |

---

## ✏️ Deleting a Transaction

1. Tap the **History** tab
2. Find the transaction
3. Tap the **✕** button on the right
4. It is deleted immediately

To fix a wrong amount — delete it and type the correct one in chat.

---

## 📅 Setting Budget Limits

1. Tap the **Budget** tab
2. Find the category (e.g. Food & Dining)
3. Type the monthly limit in the box on the right
4. Tap outside the box to save

When you go over the limit, the bar turns red and the AI warns you.

---

## 🔄 How Sync Works

Once sync is set up, everything is automatic:
- Record an expense → saves to cloud instantly
- Open the app → loads latest data from cloud
- Switch tabs → refreshes automatically
- Every 30 seconds → quietly checks for updates

You will see **"✓ Saved 09:45"** at the top to confirm it synced.

---

## ❓ Common Problems

**"API key not valid" error**
Go to Budget → Groq AI key → paste your `gsk_...` key again carefully.

**Phone and laptop not in sync**
Make sure both devices have the exact same Firebase URL. Go to Budget → ☁️ Family sync on each device and check.

**App not loading**
Check your internet. The app loads from cache if you have visited before.

**Tapping "Add to Home screen" not showing**
Use Google Chrome only — not Samsung Internet or Firefox.

---

## 💡 Tips

- You can type in natural Sri Lankan English — the AI understands
- Tap the quick buttons (Balance? / Summary / Undo) at the bottom of chat for fast answers
- The app works offline for viewing — AI chat needs internet

---

*All your data is stored privately. Nothing is shared with anyone except what the AI needs to understand your message.*
