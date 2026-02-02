# Tze Kai's Portfolio

A modern, minimalistic portfolio website inspired by Apple Intelligence design aesthetics. Built with React, TypeScript, Tailwind CSS, and Framer Motion.

**Live Site:** [https://tzekailim-SIT.github.io](https://tzekailim-SIT.github.io)

---

## ✨ Features

- **Vibrant Futuristic Design** - Dark theme with animated gradient orbs and neon glow effects
- **Apple Intelligence Aesthetic** - Clean typography, glassmorphism cards, subtle animations
- **Easy Content Editing** - All content in a single JSON file (no coding required!)
- **Project Demo Support** - Showcase GIFs/videos for your projects
- **Resume Request Form** - Protect your resume with Google Form integration
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
  "github": "https://github.com/...",
  "resumeRequestUrl": "https://forms.gle/YOUR_FORM_ID"
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

### GitHub Repositories (with Demo Support)
```json
"repositories": [
  {
    "name": "RepoName",
    "description": "Description",
    "language": "TypeScript",
    "stars": 1,
    "url": "https://github.com/...",
    "isPrivate": false,
    "featured": true,
    "demoImage": "/images/demos/repo-demo.gif",
    "demoVideo": "/images/demos/repo-demo.mp4"
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

## 🎬 Adding Project Demo GIFs/Videos

Showcase your projects with demo GIFs or videos! Here's how:

### Step 1: Create Your Demo

**Option A: Screen Recording (Recommended)**
- Use [OBS Studio](https://obsproject.com/) (free) or QuickTime (Mac)
- Record your project in action
- Export as MP4 or convert to GIF

**Option B: Convert Video to GIF**
- Use [ezgif.com](https://ezgif.com/video-to-gif) (free online tool)
- Upload your MP4 video
- Optimize for web (max 5MB recommended)

**Option C: Use LICEcap (Windows/Mac)**
- Download [LICEcap](https://www.cockos.com/licecap/)
- Record directly to GIF format

### Step 2: Upload Your Demo

1. Go to your repository on GitHub
2. Navigate to the `images/` folder
3. Create a `demos/` subfolder (click "Add file" → "Create new file" → type `demos/.gitkeep`)
4. Upload your GIF/MP4 files to `images/demos/`

### Step 3: Update config.json

Add the demo paths to your repository entry:

```json
{
  "name": "AutonomousDrone",
  "description": "Autonomous flight scripts for DJI Tello drone",
  "language": "Python",
  "stars": 1,
  "url": "https://github.com/tzekailim-SIT/AutonomousDrone",
  "isPrivate": false,
  "featured": true,
  "demoImage": "/images/demos/drone-demo.gif",
  "demoVideo": ""
}
```

**Tips:**
- Use `demoImage` for GIFs (auto-plays, no sound)
- Use `demoVideo` for MP4s (with play controls)
- Keep GIFs under 5MB for fast loading
- Use 720p resolution for best quality/size balance

---

## 📄 Setting Up Resume Request Form

Protect your resume by requiring visitors to request it through a form:

### Step 1: Create Google Form

1. Go to [forms.google.com](https://forms.google.com)
2. Click **+ Blank** to create a new form
3. Set title: "Resume Request - Tze Kai Lim"
4. Add description: "Please fill out this form to request my resume."

### Step 2: Add Form Fields

| Field | Type | Required |
|-------|------|----------|
| Full Name | Short answer | Yes |
| Email Address | Short answer (with email validation) | Yes |
| Company/Organization | Short answer | No |
| Purpose | Multiple choice (Recruitment, Networking, Academic, Other) | Yes |
| Message | Paragraph | No |

### Step 3: Get Form Link

1. Click **Send** button (top right)
2. Click the **Link icon** (chain icon)
3. Check "Shorten URL"
4. Copy the link (e.g., `https://forms.gle/XXXXXXXXX`)

### Step 4: Update config.json

```json
"profile": {
  ...
  "resumeRequestUrl": "https://forms.gle/YOUR_ACTUAL_FORM_ID"
}
```

The "Request Resume" button will automatically appear once you add a valid URL!

---

## 🖼️ How to Change Photos

### Update Profile Photo

1. Take a professional headshot (square crop works best)
2. Upload to `images/` folder in your repository
3. Update `config.json`:

```json
"profile": {
  "photo": "/images/my-new-profile.jpeg"
}
```

### Update About Section Photos

```json
"about": {
  "photos": {
    "main": {
      "src": "/images/my-main-photo.jpeg",
      "title": "Photo Title",
      "subtitle": "Photo description"
    },
    "gallery": [
      { "src": "/images/gallery-1.jpeg", "title": "Event 1" },
      { "src": "/images/gallery-2.jpeg", "title": "Event 2" }
    ]
  }
}
```

**Photo Tips:**
- Use JPEG for photos (smaller file size)
- Use PNG for screenshots with text
- Recommended sizes:
  - Profile photo: 400x400px
  - Main photo: 800x600px
  - Gallery photos: 600x400px

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
│   │       └── demos/       # ← PUT PROJECT DEMOS HERE
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
| Demo not playing | Check file format (GIF/MP4) and file size (<10MB) |
| Resume button not showing | Ensure `resumeRequestUrl` is not the placeholder value |
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
