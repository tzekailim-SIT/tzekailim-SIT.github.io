# Tze Kai's Portfolio

A modern, minimalistic portfolio website inspired by Apple Intelligence design aesthetics. Built with React, TypeScript, Tailwind CSS, and Framer Motion.

**Live Site:** [https://tzekailim-SIT.github.io](https://tzekailim-SIT.github.io)

---

## Features

- **Vibrant Futuristic Design** - Dark theme with animated gradient orbs and neon glow effects
- **Apple Intelligence Aesthetic** - Clean typography, glassmorphism cards, subtle animations
- **Responsive Layout** - Optimized for desktop, tablet, and mobile devices
- **Smooth Animations** - Powered by Framer Motion for fluid transitions
- **Google Analytics** - Built-in visitor tracking (G-YRHZF0NZPY)
- **GitHub Pages Deployment** - Free hosting with custom domain support

---

## Tech Stack

| Technology | Purpose |
|------------|---------|
| React 19 | UI Framework |
| TypeScript | Type Safety |
| Tailwind CSS 4 | Styling |
| Framer Motion | Animations |
| Vite | Build Tool |
| GitHub Pages | Hosting |

---

## Project Structure

```
portfolio/
├── client/
│   ├── public/
│   │   └── images/          # Static images
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/
│   │   │   └── Home.tsx     # Main portfolio page
│   │   ├── App.tsx          # Root component
│   │   ├── index.css        # Global styles & theme
│   │   └── main.tsx         # Entry point
│   └── index.html           # HTML template
├── dist/                    # Build output
└── README.md
```

---

## Local Development Setup

### Prerequisites

- Node.js 18+ installed
- pnpm package manager (`npm install -g pnpm`)

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/tzekailim-SIT/tzekailim-SIT.github.io.git
   cd tzekailim-SIT.github.io
   ```

2. **Install dependencies:**
   ```bash
   pnpm install
   ```

3. **Start development server:**
   ```bash
   pnpm dev
   ```

4. **Open in browser:**
   ```
   http://localhost:3000
   ```

---

## How to Edit the Portfolio

### Editing Personal Information

Open `client/src/pages/Home.tsx` and modify the following sections:

#### 1. Update Your Name & Title
```tsx
// Around line 170-180
<motion.h1 className="text-6xl ...">
  <span className="gradient-text">Your Name</span>
</motion.h1>

<motion.p className="text-xl ...">
  Your University / Company
</motion.p>
```

#### 2. Update Social Links
```tsx
// Around line 190-210
<a href="https://github.com/YOUR_USERNAME" ...>
<a href="https://www.linkedin.com/in/YOUR_PROFILE/" ...>
<a href="mailto:YOUR_EMAIL@example.com" ...>
```

#### 3. Update Projects/Repositories
```tsx
// Around line 20-35
const repositories = [
  { 
    name: "Project Name", 
    description: "Project description", 
    language: "TypeScript", 
    stars: 1, 
    url: "https://github.com/...", 
    isPrivate: false,
    featured: true  // Set to true for featured projects
  },
  // Add more projects...
];
```

#### 4. Update Skills
```tsx
// Around line 40-55
const skills = [
  { name: "Python", category: "language" },
  { name: "TypeScript", category: "language" },
  // Add more skills...
];
```

#### 5. Update Experience
```tsx
// Around line 55-75
const experiences = [
  {
    role: "Your Role",
    company: "Company Name",
    period: "2022 – 2024",
    description: "What you did...",
    highlight: "Key achievement",
  },
  // Add more experiences...
];
```

### Customizing the Design

#### Change Colors
Edit `client/src/index.css` to modify the color scheme:

```css
/* Primary gradient colors */
.gradient-text {
  background: linear-gradient(135deg, #bf5af2 0%, #5e5ce6 40%, #32d4de 70%, #ff375f 100%);
}

/* Background orb colors */
.animate-pulse-vibrant {
  /* Modify the gradient colors here */
}
```

#### Change Fonts
Edit `client/index.html` to use different Google Fonts:

```html
<link href="https://fonts.googleapis.com/css2?family=YOUR_FONT:wght@300;400;500;600;700&display=swap" rel="stylesheet" />
```

Then update `client/src/index.css`:
```css
--font-sans: 'Your Font', -apple-system, BlinkMacSystemFont, system-ui, sans-serif;
```

---

## Deployment

### Build for Production

```bash
pnpm build
```

The built files will be in `dist/public/`.

### Deploy to GitHub Pages

1. **Copy build files:**
   ```bash
   cp -r dist/public/* /path/to/your-github-pages-repo/
   ```

2. **Commit and push:**
   ```bash
   cd /path/to/your-github-pages-repo/
   git add .
   git commit -m "Update portfolio"
   git push origin main
   ```

3. **Enable GitHub Pages:**
   - Go to your repository Settings → Pages
   - Source: Deploy from branch
   - Branch: main / (root)
   - Click Save

Your site will be live at `https://YOUR_USERNAME.github.io` within a few minutes.

---

## Google Analytics

The site includes Google Analytics tracking. To use your own:

1. Create a Google Analytics 4 property at [analytics.google.com](https://analytics.google.com)
2. Get your Measurement ID (format: `G-XXXXXXXXXX`)
3. Update `client/index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-YOUR_ID"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-YOUR_ID');
</script>
```

---

## Adding New Sections

To add a new section (e.g., Blog, Certifications):

1. Add the section in `Home.tsx`:
```tsx
{/* New Section */}
<section id="new-section" className="py-32 relative">
  <div className="container mx-auto">
    <motion.div
      initial={{ opacity: 0 }}
      whileInView={{ opacity: 1 }}
      viewport={{ once: true }}
    >
      <h2 className="text-sm font-medium text-white/40 uppercase tracking-[0.3em] mb-12">
        Section Title
      </h2>
      {/* Your content here */}
    </motion.div>
  </div>
</section>
```

2. Add navigation link:
```tsx
<a href="#new-section" className="text-sm text-white/50 hover:text-white transition-colors">
  New Section
</a>
```

---

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Styles not updating | Clear browser cache or hard refresh (Ctrl+Shift+R) |
| Build fails | Run `pnpm install` to ensure all dependencies are installed |
| Images not showing | Ensure images are in `client/public/images/` and paths start with `/images/` |
| Animations laggy | Reduce number of animated elements or simplify animations |

---

## License

MIT License - Feel free to use this template for your own portfolio!

---

## Credits

- Design inspired by Apple Intelligence UI
- Icons by [Lucide](https://lucide.dev/)
- Animations by [Framer Motion](https://www.framer.com/motion/)
