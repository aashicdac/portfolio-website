# Aashi Chahal - Portfolio Website

A modern, interactive portfolio website showcasing data analytics, machine learning projects, and technical skills. Built with HTML, CSS, and JavaScript.

## 🌟 Features

- **Responsive Design** - Fully responsive across desktop, tablet, and mobile devices
- **Smooth Animations** - Scroll-based reveals, hover effects, and transitions
- **Skills Filter** - Interactive filtering system for technical skills
- **Project Showcase** - Detailed project cards with tech stacks and descriptions
- **Contact Form** - Functional contact form with validation
- **SEO Optimized** - Semantic HTML with proper meta tags
- **Fast Loading** - Optimized performance with clean code
- **Accessibility** - ARIA labels and keyboard navigation support

## 📁 Project Structure

```
portfolio/
├── index.html          # Main HTML file
├── styles.css          # Stylesheet with all styling
├── script.js           # JavaScript for interactions
├── README.md           # Documentation
└── assets/             # Folder for images and files
    ├── profile.jpg     # Your profile photo
    ├── project-maritime.jpg
    ├── project-netflix.jpg
    ├── project-nlp.jpg
    └── Aashi_Chahal_Resume.pdf
```

## 🚀 Quick Start

### 1. Download the Files

Save all three files (`index.html`, `styles.css`, `script.js`) in a folder on your computer.

### 2. Create Assets Folder

Create a folder named `assets` in the same directory as your HTML file.

### 3. Add Your Files

Add the following to the `assets` folder:

**Required:**
- `profile.jpg` - Your professional profile photo (recommended: 500x500px, square)
- `Aashi_Chahal_Resume.pdf` - Your resume PDF file

**Optional (placeholder images will work if missing):**
- `project-maritime.jpg` - Screenshot of Maritime Port Intelligence project
- `project-netflix.jpg` - Screenshot of Netflix Analytics project
- `project-nlp.jpg` - Screenshot of NLP project

### 4. Customize Content

#### Update GitHub Links
Replace `#` in the project cards with your actual GitHub repository URLs:

```html
<!-- In index.html, find project links and update -->
<a href="https://github.com/yourusername/project-name" class="project-btn">
```

#### Update Personal Information
- Email: Already set to `aashi.cdacmum.aug25@gmail.com`
- GitHub: Already set to `https://github.com/aashicdac`
- LinkedIn: Already set to `https://linkedin.com/in/aashichahal23`
- Phone: Already set to `+91 8791627341`

### 5. Test Locally

Simply open `index.html` in your web browser to preview the site.

## 🌐 Deployment to GitHub Pages

### Step 1: Create GitHub Repository

1. Go to [GitHub](https://github.com) and log in
2. Click the "+" icon in the top right and select "New repository"
3. Name it: `yourusername.github.io` (replace `yourusername` with your GitHub username)
   - Example: `aashicdac.github.io`
4. Make it **Public**
5. Click "Create repository"

### Step 2: Upload Files

**Option A: Using GitHub Web Interface (Easiest)**

1. Click "uploading an existing file"
2. Drag and drop ALL files:
   - `index.html`
   - `styles.css`
   - `script.js`
   - `assets` folder with all images
3. Scroll down and click "Commit changes"

**Option B: Using Git Command Line**

```bash
# Navigate to your portfolio folder
cd path/to/your/portfolio

# Initialize git repository
git init

# Add all files
git add .

# Commit files
git commit -m "Initial portfolio commit"

# Add remote repository
git remote add origin https://github.com/yourusername/yourusername.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Wait 2-5 minutes for deployment

### Step 4: Access Your Website

Your portfolio will be live at:
```
https://yourusername.github.io
```

Example: `https://aashicdac.github.io`

## 🎨 Customization Guide

### Change Colors

Edit the CSS variables in `styles.css`:

```css
:root {
    --color-primary: #1a5f7a;        /* Main brand color */
    --color-accent: #d4a373;         /* Accent/highlight color */
    --color-background: #0a0e17;     /* Background color */
    /* Add more customizations */
}
```

### Change Fonts

The portfolio uses:
- **Playfair Display** (headings) - Elegant serif font
- **DM Sans** (body) - Clean sans-serif font

To change fonts, update the Google Fonts link in `index.html`:

```html
<link href="https://fonts.googleapis.com/css2?family=YourFont&display=swap" rel="stylesheet">
```

Then update CSS:
```css
:root {
    --font-display: 'YourDisplayFont', serif;
    --font-body: 'YourBodyFont', sans-serif;
}
```

### Add More Projects

Copy this template in the projects section:

```html
<div class="project-card">
    <div class="project-image">
        <img src="assets/your-project.jpg" alt="Project Name">
        <div class="project-overlay">
            <span class="project-tag">New</span>
        </div>
    </div>
    <div class="project-content">
        <h3>Your Project Name</h3>
        <p>Description of your project...</p>
        <div class="project-tech">
            <span class="tech-tag">Technology 1</span>
            <span class="tech-tag">Technology 2</span>
        </div>
        <div class="project-links">
            <a href="https://github.com/..." class="project-btn">
                <i class="fab fa-github"></i> View Code
            </a>
        </div>
    </div>
</div>
```

### Add More Skills

Copy this template in the skills section:

```html
<div class="skill-card" data-category="category-name">
    <div class="skill-icon">
        <i class="fas fa-icon-name"></i>
    </div>
    <h3>Skill Name</h3>
    <p>Description</p>
    <div class="skill-level">
        <div class="skill-bar" style="--skill-width: 85%"></div>
    </div>
</div>
```

## 📧 Contact Form Setup

The contact form currently shows a simulated submission. To make it functional:

### Option 1: EmailJS (Recommended - Free)

1. Sign up at [EmailJS](https://www.emailjs.com/)
2. Create an email service and template
3. Add this before `</body>` in `index.html`:
   ```html
   <script src="https://cdn.jsdelivr.net/npm/@emailjs/browser@3/dist/email.min.js"></script>
   <script>
       emailjs.init('YOUR_PUBLIC_KEY');
   </script>
   ```
4. Uncomment the EmailJS code in `script.js`

### Option 2: Formspree

1. Sign up at [Formspree](https://formspree.io/)
2. Create a form and get your form endpoint
3. Update the form in `index.html`:
   ```html
   <form action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
   ```

### Option 3: Netlify Forms

If deploying to Netlify, add `netlify` attribute:
```html
<form name="contact" method="POST" data-netlify="true">
```

## 🔍 SEO Optimization

### Update Meta Tags

In `index.html`, update:

```html
<meta name="description" content="Your custom description">
<meta name="keywords" content="Your, Custom, Keywords">
<meta property="og:title" content="Your Title">
<meta property="og:description" content="Your Description">
```

### Add Google Analytics

1. Get your Google Analytics tracking ID
2. Add before `</head>` in `index.html`:

```html
<!-- Google Analytics -->
<script async src="https://www.googletagmanager.com/gtag/js?id=GA_MEASUREMENT_ID"></script>
<script>
    window.dataLayer = window.dataLayer || [];
    function gtag(){dataLayer.push(arguments);}
    gtag('js', new Date());
    gtag('config', 'GA_MEASUREMENT_ID');
</script>
```

## 🖼️ Image Recommendations

### Profile Photo
- **Format:** JPG or PNG
- **Size:** 500x500px (square)
- **Quality:** High resolution, professional
- **Background:** Clean, plain background or transparent

### Project Screenshots
- **Format:** JPG or PNG
- **Dimensions:** 1200x800px (3:2 ratio)
- **Quality:** High quality, clear visuals
- **Content:** Show main features/UI of your projects

### Optimization
Use tools like [TinyPNG](https://tinypng.com/) to compress images without losing quality.

## 🛠️ Technologies Used

- **HTML5** - Semantic markup
- **CSS3** - Modern styling with custom properties
- **JavaScript (ES6+)** - Interactive features
- **Font Awesome** - Icons
- **Google Fonts** - Typography

## 📱 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Mobile browsers

## 🐛 Troubleshooting

### Images Not Showing
- Check that images are in the `assets` folder
- Verify image file names match exactly (case-sensitive)
- Ensure images are in JPG, PNG, or WebP format

### Contact Form Not Working
- Implement one of the contact form solutions above
- Check browser console for JavaScript errors

### GitHub Pages Not Deploying
- Wait 5-10 minutes after enabling Pages
- Check that repository is public
- Ensure `index.html` is in the root directory

### Styles Not Applying
- Clear browser cache (Ctrl+Shift+R or Cmd+Shift+R)
- Verify `styles.css` and `script.js` are in the same folder as `index.html`

## 📄 License

This portfolio template is free to use for personal projects. Feel free to customize it for your needs!

## 🤝 Credits

- Icons: [Font Awesome](https://fontawesome.com/)
- Fonts: [Google Fonts](https://fonts.google.com/)
- Design inspiration: Modern portfolio best practices

## 📞 Support

For questions or issues:
- Email: aashi.cdacmum.aug25@gmail.com
- GitHub: [@aashicdac](https://github.com/aashicdac)

---

**Built with ❤️ by Aashi Chahal**

*Last Updated: February 2025*
