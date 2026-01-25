# ◈ GHOSTLINK APP REGISTRY

This repository is the official community-driven marketplace for **GhostLink**. It allows developers to publish standalone HTML applications, tools, and games that users can install directly into their personal GhostLink dashboard.

---

## How It Works
1. **The Registry**: The `apps.json` file acts as a serverless database containing the metadata for every app in the store.
2. **The Connection**: The GhostLink UI fetches this raw JSON data from GitHub to display the marketplace.
3. **The Installation**: When a user clicks "Install," the app data is saved to their browser's `localStorage`, making it accessible even after refreshing the page.

---

## For Developers: How to Publish
Adding your app to the GhostLink marketplace is free and open to everyone!

### 1. Host Your Application
Your app must be a standalone HTML file. You can host it using:
* **GitHub Pages** (Recommended)
* **JSdeliver**
* **Vercel** or **Netlify**

### 2. Fork & Edit
1. **Fork** this repository to your own account.
2. Open the `apps.json` file.
3. Add a new object to the `apps` array using the template below.

### 3. Submission Template
Copy and fill out this structure into `apps.json`:

'''json
{
  "name": "Your App Name",
  "author": "Your GitHub Name",
  "description": "A short, one-sentence description of what your app does.",
  "url": "[https://your-username.github.io/your-repo/index.html] or jsdeliver link",
  "svg": "<svg viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2'>your svg code here</svg>"
}

### 4. Open a Pull Request
Once you've saved your changes to your fork, open a Pull Request to the main repository. After a brief security review, your app will be merged and instantly go live for all GhostLink users.
