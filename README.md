# AgentBee Admin — Information Updates

A password-protected admin tool for posting Knowledge Base and
Community of Practice notifications to client institution feeds.

## First-time setup

### 1. Fill in config.js

Open `config.js` and replace all three placeholder values:

```js
const SUPABASE_URL  = 'https://YOUR_PROJECT_REF.supabase.co';
const SUPABASE_ANON = 'YOUR_ANON_KEY';
const ADMIN_PASS    = 'CHANGE_ME_123'; // ← change this before deploying
```

`config.js` is gitignored — never committed to GitHub, never overwritten by future zips.

### 2. Deploy to Vercel

- Push folder contents to a new GitHub repo named `agentbee-admin`
- Import into Vercel → Deploy
- Access at your Vercel URL (no need to embed anywhere)

## How to use

1. Open the URL in your browser
2. Enter your admin passphrase
3. Select category: **Knowledge Base** or **Community of Practice**
4. Enter a description (shown in the feed, max 200 chars)
5. Enter the link URL (the Circle space URL or article URL)
6. Choose to send to **all client institutions** or **select specific ones**
7. Click **Post update**

## Updating (future zips from Claude)

Replace `index.html`, `vercel.json`, `README.md` only.
Leave `config.js` and `.gitignore` untouched.
