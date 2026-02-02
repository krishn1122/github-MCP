# 📸 Creative Lens - Photographer & Influencer Portfolio

A stunning, interactive, and fully responsive portfolio website designed for photographers and social media influencers. Built with modern web technologies and featuring a social media-inspired theme with beautiful animations and interactive elements.

![Portfolio Preview](https://img.shields.io/badge/Status-Live-success?style=for-the-badge)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

## ✨ Features

### 🎨 Design & UI
- **Social Media Theme**: Instagram-inspired gradient colors and modern design
- **Fully Responsive**: Perfect display on all devices (mobile, tablet, desktop)
- **Dark Mode**: Eye-friendly dark theme throughout
- **Smooth Animations**: Scroll animations, hover effects, and transitions
- **Custom Cursor**: Interactive custom cursor for desktop users

### 📱 Sections

1. **Hero Section**
   - Animated title with gradient text
   - Real-time statistics counter (followers, projects, likes)
   - Floating social media cards with animations
   - Call-to-action buttons

2. **About Section**
   - Professional bio with image
   - Social media links overlay
   - Skills showcase with icons
   - Smooth reveal animations

3. **Gallery Section**
   - Filterable portfolio grid (All, Portrait, Landscape, Product, Lifestyle)
   - Interactive image cards with hover effects
   - Social engagement stats (likes, comments)
   - Expandable image view

4. **Social Media Section**
   - Platform-specific cards (Instagram, YouTube, TikTok, Twitter)
   - Real-time statistics display
   - Direct links to social profiles
   - Live feed widget showing recent posts

5. **Contact Section**
   - Interactive contact form with validation
   - Animated form inputs
   - Contact information cards
   - Social media quick links

6. **Footer**
   - Quick navigation links
   - Services list
   - Social media icons
   - Copyright information

### 🚀 Interactive Features

- **Smooth Scrolling**: Seamless navigation between sections
- **Scroll Animations**: Elements animate into view as you scroll
- **Gallery Filtering**: Dynamic filtering with smooth transitions
- **Counter Animation**: Numbers count up when visible
- **Form Validation**: Real-time form validation with visual feedback
- **Back to Top Button**: Quick navigation to top of page
- **Mobile Menu**: Responsive hamburger menu for mobile devices
- **Custom Cursor**: Interactive cursor that responds to hover states
- **Parallax Effects**: Subtle parallax scrolling on background elements

## 🛠️ Technologies Used

- **HTML5**: Semantic markup and structure
- **CSS3**: Modern styling with Flexbox and Grid
- **JavaScript (Vanilla)**: Interactive functionality and animations
- **Font Awesome 6.4.0**: Icon library for social media and UI icons
- **Google Fonts**: Poppins and Playfair Display fonts
- **Unsplash**: High-quality placeholder images

## 📦 Installation & Setup

### Quick Start

1. **Clone or Download** the repository:
   ```bash
   git clone https://github.com/krishn1122/github-MCP.git
   cd github-MCP
   ```

2. **Open the project**:
   - Simply open `index.html` in your web browser
   - Or use a local development server (recommended)

### Using a Local Server

#### Option 1: VS Code Live Server
1. Install the "Live Server" extension in VS Code
2. Right-click on `index.html`
3. Select "Open with Live Server"

#### Option 2: Python HTTP Server
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000
```
Then open `http://localhost:8000` in your browser

#### Option 3: Node.js HTTP Server
```bash
npx http-server
```

## 🎨 Customization Guide

### 1. Personal Information

Edit `index.html` to update:
- Name and title in the hero section
- About section bio and description
- Contact information (email, phone, location)
- Social media links

### 2. Colors & Theme

Edit `styles.css` CSS variables in `:root`:
```css
:root {
    --primary-color: #e1306c;        /* Main accent color */
    --secondary-color: #405de6;      /* Secondary accent */
    --dark-bg: #0a0a0a;              /* Background color */
    --card-bg: #1a1a1a;              /* Card background */
    --text-primary: #ffffff;         /* Primary text */
    --text-secondary: #b0b0b0;       /* Secondary text */
}
```

### 3. Images

Replace placeholder images:
- Update image URLs in `index.html`
- Use your own photography portfolio images
- Recommended image sizes:
  - Hero images: 1920x1080px
  - Gallery images: 800x800px
  - About image: 600x800px
  - Feed images: 400x400px

### 4. Social Media Stats

Update statistics in `index.html`:
```html
<h3 class="stat-number" data-target="250">0</h3>
```
Change `data-target` to your actual numbers

### 5. Gallery Categories

Add or modify categories in the filter buttons and gallery items:
```html
<button class="filter-btn" data-filter="your-category">
    <i class="fas fa-icon"></i> Your Category
</button>

<div class="gallery-item" data-category="your-category">
    <!-- Image content -->
</div>
```

## 📱 Social Media Integration

### Connecting Your Accounts

1. **Instagram**: Replace `#` in social card links with your Instagram profile URL
2. **YouTube**: Update with your YouTube channel URL
3. **TikTok**: Add your TikTok profile link
4. **Twitter**: Insert your Twitter/X profile URL
5. **LinkedIn**: Add your LinkedIn profile (in contact section)

### Live Feed Widget

To display real Instagram posts:
- Use Instagram's official embed API
- Or integrate with third-party services like Juicer or SnapWidget
- Replace placeholder images with actual feed URLs

## 🔧 Advanced Customization

### Adding New Sections

1. Create HTML structure in `index.html`
2. Add corresponding styles in `styles.css`
3. Update navigation menu with new section link
4. Add scroll animations in `script.js` if needed

### Modifying Animations

Edit animation properties in `styles.css`:
```css
@keyframes yourAnimation {
    from { /* start state */ }
    to { /* end state */ }
}
```

### Form Integration

Connect the contact form to a backend service:
- **EmailJS**: Free email service for static sites
- **Formspree**: Simple form endpoint
- **Netlify Forms**: If hosting on Netlify
- **Custom Backend**: Node.js, PHP, or other server-side solution

Example with EmailJS:
```javascript
// In script.js, replace the setTimeout with:
emailjs.send("service_id", "template_id", formData)
    .then(() => {
        // Success message
    });
```

## 🌐 Deployment

### GitHub Pages

1. Push your code to GitHub
2. Go to repository Settings → Pages
3. Select branch (main) and folder (root)
4. Your site will be live at `https://yourusername.github.io/repo-name`

### Netlify

1. Drag and drop your project folder to [Netlify](https://netlify.com)
2. Or connect your GitHub repository
3. Site will be live instantly with custom domain option

### Vercel

1. Install Vercel CLI: `npm i -g vercel`
2. Run `vercel` in project directory
3. Follow prompts for deployment

## 📊 Performance Optimization

- **Images**: Compress images using TinyPNG or ImageOptim
- **Lazy Loading**: Add `loading="lazy"` to images
- **Minification**: Minify CSS and JS for production
- **CDN**: Use CDN for Font Awesome and Google Fonts
- **Caching**: Configure browser caching for static assets

## 🐛 Browser Support

- ✅ Chrome (latest)
- ✅ Firefox (latest)
- ✅ Safari (latest)
- ✅ Edge (latest)
- ✅ Opera (latest)
- ⚠️ IE11 (limited support, some features may not work)

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 💡 Tips for Photographers & Influencers

1. **High-Quality Images**: Use professional, high-resolution photos
2. **Consistent Branding**: Match colors to your personal brand
3. **Regular Updates**: Keep your portfolio and stats current
4. **SEO Optimization**: Add meta tags and descriptions
5. **Analytics**: Integrate Google Analytics to track visitors
6. **Social Proof**: Display real testimonials and collaborations
7. **Call-to-Actions**: Make it easy for clients to contact you

## 📞 Support

For questions or support, please:
- Open an issue on GitHub
- Contact via email: hello@creativelens.com
- Follow on social media for updates

## 🎉 Acknowledgments

- Font Awesome for amazing icons
- Unsplash for beautiful stock photos
- Google Fonts for typography
- The web development community for inspiration

---

**Made with ❤️ for photographers and content creators**

🌟 If you like this project, please give it a star on GitHub!
