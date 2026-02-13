# Corina Cuevas Coaching Website

A professional, mobile-responsive coaching website built with HTML, CSS, and JavaScript.

## 📁 Files Included

1. **index.html** - Main HTML structure
2. **style.css** - Custom styling with brand colors
3. **script.js** - Interactive JavaScript functionality

## 🎨 Design Features

### Brand Colors
- Background: #fdf7eb (warm cream)
- Gold Accent: #e8cba4
- Primary Dark: #1e2a35
- Coral Accent: #d96a53

### Typography
- Headers: EB Garamond (elegant serif)
- Body: Inter (clean sans-serif)

### Mobile-Responsive
- Hamburger menu for mobile devices
- Responsive grid layouts
- Touch-friendly navigation
- Optimized for all screen sizes

## 🚀 Getting Started

### Basic Setup
1. Place all three files in the same folder
2. Open `index.html` in a web browser
3. The website will work immediately!

### Customization Needed

#### 1. Calendly Link
Replace the placeholder in `index.html` (line ~149):
```html
<a href="#" class="btn-primary">Book Your Call</a>
```
Change to:
```html
<a href="https://calendly.com/your-link" target="_blank" class="btn-primary">Book Your Call</a>
```

#### 2. Contact Form Backend
The contact form currently shows an alert. To make it functional, integrate with:

**Option A: Formspree (Recommended - Easy & Free)**
1. Go to https://formspree.io/
2. Create a free account
3. Get your form endpoint
4. Update `script.js` (line ~40):
```javascript
fetch('https://formspree.io/f/YOUR_FORM_ID', {
    method: 'POST',
    body: formData,
    headers: {
        'Accept': 'application/json'
    }
}).then(response => {
    if (response.ok) {
        alert('Thank you! Your message has been sent.');
        contactForm.reset();
    }
});
```

**Option B: EmailJS**
1. Go to https://www.emailjs.com/
2. Set up email service
3. Follow their documentation to integrate

**Option C: Google Forms**
Replace the contact form with an embedded Google Form

#### 3. Add Credly Badges (Optional)
1. Get your Credly badge embed codes
2. Add a new section in `index.html` after credentials:
```html
<div class="badges">
    <h3>Certifications</h3>
    <div class="badge-container">
        <!-- Paste Credly badge codes here -->
    </div>
</div>
```

## 📱 Mobile Features

- **Responsive Navigation**: Hamburger menu appears on screens < 768px
- **Touch-Optimized**: All buttons and links sized for easy tapping
- **Fluid Layouts**: Content adapts seamlessly to any screen size
- **Readable Typography**: Font sizes adjust for mobile readability

## 🔧 Technical Features

1. **Smooth Scrolling**: Click navigation links for smooth page transitions
2. **Fade-in Animations**: Sections animate as you scroll
3. **Sticky Navigation**: Header stays visible while scrolling
4. **Form Validation**: Built-in HTML5 form validation
5. **Cross-browser Compatible**: Works on all modern browsers

## 📝 Content Sections

1. **Hero** - Main headline and CTA
2. **Introduction** - Coaching philosophy
3. **Is Coaching Right for You?** - Self-assessment items
4. **Services** - 4 coaching offerings
5. **Testimonials** - 5 client testimonials
6. **About** - Biography, approach, and credentials
7. **Contact** - Dual contact options (scheduling + form)
8. **Footer** - Copyright and email

## 🎯 SEO & Performance

- Semantic HTML5 structure
- Meta descriptions included
- Fast loading times
- Mobile-first approach
- Accessibility features (ARIA labels)

## 🌐 Deployment Options

### Option 1: Netlify (Recommended - Free)
1. Go to https://www.netlify.com/
2. Drag and drop your folder
3. Get a free custom URL

### Option 2: GitHub Pages (Free)
1. Create GitHub account
2. Create repository
3. Upload files
4. Enable GitHub Pages in settings

### Option 3: Traditional Web Hosting
Upload all three files to your hosting provider via FTP

## 📧 Contact Information

Email: corinacuevascoaching@gmail.com
LinkedIn: https://www.linkedin.com/in/corina-cuevas/

## 🔄 Future Enhancements

Consider adding:
- Blog section for thought leadership
- Resource downloads (PDF guides)
- Video testimonials
- Calendar integration
- Analytics (Google Analytics)
- Newsletter signup
- Social media feed integration

## 💡 Tips

1. **Test on Real Devices**: Check how it looks on actual phones/tablets
2. **Optimize Images**: Compress any images before adding (use TinyPNG)
3. **Regular Updates**: Keep testimonials and credentials current
4. **Track Performance**: Add Google Analytics to monitor visitors
5. **Backup Files**: Keep copies of your website files

## 🐛 Troubleshooting

**Menu not working on mobile?**
- Check that script.js is loaded properly
- Clear browser cache

**Form not submitting?**
- Integrate with Formspree or EmailJS (see instructions above)

**Styling looks wrong?**
- Verify style.css is in the same folder as index.html
- Check for typos in file names

**Fonts not loading?**
- Ensure internet connection (fonts load from Google Fonts)
- Check browser console for errors

---

Built with care for Corina Cuevas Coaching • 2026