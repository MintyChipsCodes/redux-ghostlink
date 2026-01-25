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

### 2. Create a JSON file with the following format
```json
{
  "id": "unique_id_123",
  "name": "My Cool App",
  "author": "YourGitHubName",
  "description": "What your app does in one sentence.",
  "url": "https://your-username.github.io/your-app/",
  "svg": "<svg viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2'><circle cx='12' cy='12' r='10'/></svg>"
}
```
### 3. Fork & Upload

Fork this repository.
Navigate into the /apps folder.
Upload your your-app-name.json file into that folder.
Submit a Pull Request.
Once merged, your app will automatically appear in the GhostLink Marketplace!
