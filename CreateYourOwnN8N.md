# 🌐 **What is n8n?**

n8n is an **open-source workflow automation tool**—like Zapier, Make, or IFTTT—but more powerful because it is:

* 🌍 Self-hostable
* 🔗 Unlimited workflows
* 🤖 Supports AI agents, APIs, databases, etc.
* 🧩 400+ integrations
* 🔓 Free & open-source

Your personal n8n instance = **your own automation server**.

---

# 🚀 **How to Create Your Own n8n (100% Free) Using Render**

This will create a URL like:
👉 **[https://your-app-name.onrender.com](https://your-app-name.onrender.com)**

Just like your:
👉 **[https://n8n-cg6a.onrender.com](https://n8n-cg6a.onrender.com)**

---

# 🟦 **Step 1: Create Render Account**

Go to: [https://render.com](https://render.com)
Sign up using Google or GitHub.

---

# 🟧 **Step 2: Create New Web Service**

1. Click **New +**
2. Choose **Web Service**
3. Select **Public Git Repo**
4. Paste this n8n official repository:

```
https://github.com/n8n-io/n8n
```

---

# 🟩 **Step 3: Configure Render Settings**

| Setting           | Value                              |
| ----------------- | ---------------------------------- |
| **Name**          | n8n-yourname (any)                 |
| **Runtime**       | Docker                             |
| **Region**        | Singapore / India (lowest latency) |
| **Instance type** | Free                               |

Scroll down ⬇️

---

# 🟪 **Step 4: Add Environment Variables (IMPORTANT)**

Add these:

### 🔐 1. `N8N_BASIC_AUTH_ACTIVE=true`

### 🔐 2. `N8N_BASIC_AUTH_USER=admin`

### 🔐 3. `N8N_BASIC_AUTH_PASSWORD=yourpassword`

→ This protects your n8n from public access.

### 🌍 4. `WEBHOOK_TUNNEL_URL`

Set it to your future domain format:

```
https://n8n-yourname.onrender.com
```

### 🟡 5. (Optional) Database

For beginners, skip.

Then click **Deploy Web Service**.

---

# 💠 **Step 5: Wait 2–3 Minutes**

Render builds Docker → deploys → gives you your own URL:

👉 [https://n8n-yourname.onrender.com](https://n8n-yourname.onrender.com)

Open it → login using your username & password.

🎉 **Congratulations! Your n8n is live.**

---

# 🔒 **Step 6: Secure Your n8n (VERY IMPORTANT)**

Add more environment variables later (recommended):

```
N8N_PROTOCOL=https
N8N_HOST=n8n-yourname.onrender.com
N8N_PORT=5678
```

---

# 🛠️ **Step 7: Create Your First Workflow**

Once inside your n8n instance:

### Example: Simple AI Chatbot Workflow

Nodes:

1. **When Chat Message Received (Trigger)**
2. **AI Agent**
3. **Google Gemini Model**
4. **Simple Memory**
5. **Respond**

This is exactly what you built in your screenshot.

You can also automate:

* WhatsApp bot
* Gmail auto-replies
* Google Sheets automations
* Cron jobs
* APIs
* Instagram / LinkedIn posting
* Database workflows
* AI-generated content

---

# 🔥 **Bonus: Add Your Custom Domain**

If you own a domain, you can map:

👉 [https://automation.yourdomain.com](https://automation.yourdomain.com) → your Render n8n

Using:

* CNAME
* SSL auto-enabled by Render

---

# 🧠 Want an even more powerful setup?

I can help you deploy:

✅ n8n on VPS (DigitalOcean, Hetzner)
— Faster, unlimited workflows

✅ n8n with PostgreSQL
— More stable for big automation

✅ n8n with Docker Compose
— Perfect for production

