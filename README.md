# VS · Resume Hub — Landing Page

> Personal resume hub & link-in-bio landing page for **Vinayak Sharma**  
> Live at → [links.vinayaksharma.dpdns.org](https://links.vinayaksharma.dpdns.org)

---

## 📁 Project Structure

```
resume_hub_landing_page/
├── index.html          # Main landing page (Resume Hub)
├── qr-generator.html   # QR Code generator utility
├── CNAME               # Custom subdomain config
├── .github/
│   └── workflows/
│       └── deploy.yml  # GitHub Actions CI/CD pipeline
└── README.md
```

---

## 🚀 Deployment

This project auto-deploys to **GitHub Pages** via GitHub Actions on every push to `main`.

### How it works

1. Push any change to `main`
2. GitHub Actions runs the `deploy.yml` workflow
3. The site goes live at your custom subdomain automatically

---

## 🌐 Custom Subdomain Setup

The `CNAME` file points GitHub Pages to your custom subdomain.

### DNS Configuration (in your domain registrar / DuckDNS)

Add a **CNAME record**:

| Type  | Host    | Value                              |
| ----- | ------- | ---------------------------------- |
| CNAME | `links` | `<your-github-username>.github.io` |

> Replace `<your-github-username>` with your actual GitHub username.

---

## ✏️ Updating Your Info

All personal data lives in one place inside `index.html`:

```js
const MY = {
  name: 'Vinayak Sharma',
  title: 'Associate Engineer - IIoT',
  phone: '+91 7975524393',
  email: 'vvsharma999@gmail.com',
  portfolio: 'https://vinayaksharma.dpdns.org/',
  github: 'https://github.com/Vinayaksharma17',
  video: 'https://youtube.com/shorts/nhTyncMMm0s',
  linkedin: 'https://www.linkedin.com/in/vinayak-sharma17/',
}
```

Edit those values and push — the site updates automatically.

---

## 🛠️ Local Development

No build tools needed. Just open in your browser:

```bash
open index.html
```

Or use the VS Code Live Server extension for hot-reload.

---

## 📄 License

MIT — feel free to fork and adapt for your own use.
