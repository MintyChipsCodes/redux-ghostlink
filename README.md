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
* **GitHub** (recomended, raw file url or just file url)
* **JSdeliver link**
* **Raw HTML** (MUST BE CONVERTED TO A SINGLE LINE)

### 2. Create a JSON file with the following format
For a Github file:
```json
{
  "name": "My Cool App",
  "author": "YourGitHubName",
  "description": "What your app does in one sentence.",
  "url": "https://raw.githubusercontent.com/yourusername/repositoryname/main/something.html",
  "svg": "<svg viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2'><your svg code ></svg>"
}
```
For a raw HTML file:
```json
{
  "name": "My Cool App",
  "author": "YourGitHubName",
  "description": "What your app does in one sentence.",
  "url": "data:text/html;charset=utf-8,<!DOCTYPE html><html lang=\"en\">...HTML must be in this...</html>",
  "svg": "<svg viewBox='0 0 24 24' fill='none' stroke='currentColor' stroke-width='2'><your svg code ></svg>"
}
```
### 3. Fork & Upload

Fork this repository.
Navigate into the /apps folder.
Upload your your-app-name.json file into that folder.
Submit a Pull Request.
Your file will be reviewed. Absolutely no malware, phishing, or stealing users data.
Once merged, your app will automatically appear in the GhostLink Marketplace!
