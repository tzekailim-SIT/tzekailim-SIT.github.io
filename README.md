# Tze Kai's Portfolio

A modern, minimalistic portfolio website inspired by Apple Intelligence design aesthetics. Built with React, TypeScript, Tailwind CSS, and Framer Motion.

**Live Site:** [https://tzekailim-SIT.github.io](https://tzekailim-SIT.github.io)

---

## ✨ Features

- **Vibrant Futuristic Design** - Dark theme with animated gradient orbs and neon glow effects
- **Apple Intelligence Aesthetic** - Clean typography, glassmorphism cards, subtle animations
- **Easy Content Editing** - All content in a single JSON file (no coding required!)
- **Responsive Layout** - Optimized for desktop, tablet, and mobile devices
- **Smooth Animations** - Powered by Framer Motion for fluid transitions
- **Google Analytics** - Built-in visitor tracking
- **GitHub Pages Deployment** - Free hosting with custom domain support

---

## ✏️ Easy Content Editing (No Coding Required!)

All portfolio content is stored in a single JSON file: **`config.json`**

You can edit this file directly on GitHub to update your portfolio instantly!

### How to Edit on GitHub (Easiest Method)

1. Go to your repository: [https://github.com/tzekailim-SIT/tzekailim-SIT.github.io](https://github.com/tzekailim-SIT/tzekailim-SIT.github.io)
2. Click on `config.json`
3. Click the **pencil icon** (Edit this file)
4. Make your changes
5. Click **Commit changes**
6. Your site will update automatically in 1-2 minutes!

---

## 📝 What You Can Edit in config.json

### Profile Information
```json
"profile": {
  "name": "Tze Kai",
  "fullName": "Tze Kai Lim",
  "title": "Your title here",
  "tagline": "Computing Science · Aviation · Innovation",
  "bio": "Your bio paragraph...",
  "photo": "/images/tzekai-profile.jpeg",
  "email": "your@email.com",
  "linkedin": "https://linkedin.com/in/...",
  "github": "https://github.com/..."
}
```

### Statistics
```json
"stats": {
  "connections": "500+",
  "followers": "718",
  "certifications": "11",
  "repositories": "21"
}
```

### About Section
```json
"about": {
  "journey": "First paragraph of your story...",
  "journeyExtended": "Second paragraph...",
  "achievements": [
    { "text": "Achievement 1", "color": "cyan" },
    { "text": "Achievement 2", "color": "purple" }
  ],
  "photos": {
    "main": {
      "src": "/images/your-photo.jpeg",
      "title": "Photo Title",
      "subtitle": "Photo subtitle"
    },
    "gallery": [
      { "src": "/images/photo1.jpeg", "title": "Title 1" },
      { "src": "/images/photo2.jpeg", "title": "Title 2" }
    ]
  }
}
```

### Education
```json
"education": [
  {
    "degree": "BSc (Hons) Computing Science",
    "school": "SIT × University of Glasgow",
    "period": "2024 – 2027"
  }
]
```

### Work Experience
```json
"experiences": [
  {
    "role": "Job Title",
    "company": "Company Name",
    "period": "Jan 2025 – Present",
    "description": "What you did...",
    "highlight": "Key achievement",
    "icon": "briefcase"
  }
]
```

**Available icons:** `plane`, `shield`, `briefcase`, `code`, `rocket`, `cloud`, `database`, `cpu`, `bot`, `users`

### Skills
```json
"skills": [
  {
    "name": "Category Name",
    "icon": "code",
    "color": "from-purple-500 to-violet-500",
    "skills": ["Skill 1", "Skill 2", "Skill 3"]
  }
]
```

### Certifications
```json
"certifications": [
  { "name": "Certification Name", "issuer": "Issuing Org", "date": "Oct 2024" }
],
"additionalCertificationsCount": 6
```

### Notable Projects
```json
"notableProjects": [
  {
    "name": "Project Name",
    "description": "What you built",
    "association": "Company/School"
  }
]
```

### GitHub Repositories
```json
"repositories": [
  {
    "name": "RepoName",
    "description": "Description",
    "language": "TypeScript",
    "stars": 1,
    "url": "https://github.com/...",
    "isPrivate": false,
    "featured": true
  }
]
```

### Contact & Footer
```json
"contact": {
  "heading": "Let's Connect",
  "description": "Your contact message..."
},
"footer": {
  "copyright": "© 2025 Your Name. Built with passion."
}
```

---

## 🖼️ How to Change Photos

1. **Upload new photos** to the `images/` folder in your repository
2. **Update the path** in `config.json` to point to your new image
3. Commit changes

**Supported formats:** `.jpeg`, `.jpg`, `.png`, `.webp`

**Example:**
```json
"photo": "/images/my-new-photo.jpeg"
```

---

## 💻 Local Development Setup

### Prerequisites
- Node.js 18+ installed
- pnpm package manager (`npm install -g pnpm`)

### Installation

```bash
# Clone the repository
git clone https://github.com/tzekailim-SIT/tzekailim-SIT.github.io.git
cd tzekailim-SIT.github.io

# Install dependencies
pnpm install

# Start development server
pnpm dev
```

The site will be available at `http://localhost:3000`

### Building for Production

```bash
pnpm build
```

Output files will be in the `dist/public/` folder.

---

## 📁 Project Structure

```
├── client/
│   ├── public/
│   │   ├── config.json      # ← EDIT THIS FILE for content changes
│   │   └── images/          # ← PUT YOUR PHOTOS HERE
│   ├── src/
│   │   ├── pages/
│   │   │   └── Home.tsx     # Main page component
│   │   ├── hooks/
│   │   │   └── useConfig.ts # Config loader hook
│   │   └── index.css        # Styles and animations
│   └── index.html           # HTML template
├── README.md                # This file
└── package.json             # Dependencies
```

---

## 🎨 Customizing the Design (Advanced)

### Change Colors
Edit `client/src/index.css` to modify the color scheme:

```css
/* Primary gradient colors */
.gradient-text {
  background: linear-gradient(135deg, #bf5af2 0%, #5e5ce6 40%, #32d4de 70%, #ff375f 100%);
}
```

### Change Fonts
Edit `client/index.html` to use different Google Fonts:

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR_FONT:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
```

---

## 🚀 Deployment

This site is automatically deployed via GitHub Pages whenever you push to the `main` branch.

**To manually deploy:**
1. Make your changes
2. Commit and push to `main`
3. GitHub Pages will automatically rebuild (1-2 minutes)

---

## 🔧 Troubleshooting

| Issue | Solution |
|-------|----------|
| Changes not appearing | Wait 1-2 minutes, then hard refresh (Ctrl+Shift+R) |
| JSON error | Validate your JSON at [jsonlint.com](https://jsonlint.com) |
| Images not loading | Ensure path starts with `/images/` and file exists |
| Build fails | Run `pnpm install` to ensure dependencies are installed |

---

## 📄 License

MIT License - Feel free to use this template for your own portfolio!

---

## 🙏 Credits

Built with:
- React 19 & TypeScript
- Tailwind CSS 4
- Framer Motion
- Lucide Icons

Design inspired by Apple Intelligence aesthetic.
