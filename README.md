# IBM Bob – Student Resources Page

A simple static HTML page that collects all important links and downloadable files for students in the **Edunet Foundation × IBM Bob** programme.

## 🔗 Live Site

Once deployed to GitHub Pages, the site will be available at:
```
https://<your-github-username>.github.io/<repo-name>/
```

## 📁 Structure

```
student-resources/
├── index.html          ← Main page (links + downloads)
└── files/
    └── important-links.txt   ← Plain-text copy of all links
```

## 🚀 Hosting on GitHub Pages

1. Push this folder (or the whole repo) to GitHub.
2. Go to **Settings → Pages** in your repository.
3. Under **Source**, choose `main` branch and `/` (root) or `/docs` folder.
4. Click **Save** — your page will be live in ~60 seconds.

## ➕ Adding More Links

Open `index.html` and copy-paste a new `<a class="card">` block inside the `card-grid` div:

```html
<a class="card" href="https://example.com" target="_blank" rel="noopener">
  <span class="card-title">Title Here</span>
  <span class="card-desc">Short description for students.</span>
</a>
```

## ➕ Adding More Files

1. Drop the file into the `files/` folder.
2. Add a new `<li>` entry in the **Files & Downloads** section of `index.html`:

```html
<li>
  <span class="icon">📄</span>
  <div>
    <a href="files/your-file.pdf" download>your-file.pdf</a>
    <div class="meta">Brief description of the file</div>
  </div>
</li>
```
