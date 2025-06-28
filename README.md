# Rubixvi Landing Page

A modern, single-page website for Rubixvi - a healthcare technology startup focused on re-imagining global healthcare.

## 🌐 Live Site

Visit: [www.rubixvi.com](https://www.rubixvi.com)

## 📁 Project Structure

```
rubix6-launch/
├── index.html          # Production landing page (GitHub Pages)
├── index-dev.html      # Development version with enhanced features
├── styles.css          # Shared CSS styles
├── jobs.json          # Job listings data (for dev version)
├── rubixvi_logo.png   # Company logo
├── favicon.ico        # Website favicon
├── CNAME              # GitHub Pages custom domain
└── CLAUDE.md          # Development documentation
```

## 🚀 Features

### Production Version (`index.html`)
- Simple, clean landing page
- Company branding and basic information

### Development Version (`index-dev.html`)
- **Hero Section**: Logo, tagline, and call-to-action
- **Feature Cards**: About, Vision, Join Us, Contact, Connect
- **Careers Section**: Dynamic job listings with expandable details
- **Animations**: Smooth scroll animations powered by anime.js
- **Interactive Elements**: 
  - Floating back-to-top button with section navigation
  - Expandable job cards with structured content
  - Smooth scrolling between sections

## 💻 Local Development

### Quick Start

The simplest way to view the development version:

1. **Clone the repository**
   ```bash
   git clone https://github.com/rubix6-n3/rubix6-launch.git
   cd rubix6-launch
   ```

2. **Start a local server**
   ```bash
   # Using Python 3 (recommended)
   python3 -m http.server 8000
   
   # Or using Python 2
   python -m SimpleHTTPServer 8000
   
   # Alternative with Node.js (if available)
   npx serve .
   ```

3. **Open in browser**
   ```
   http://localhost:8000/index-dev.html
   ```

### Why Use a Local Server?

When opening HTML files directly in a browser (`file://` protocol), modern browsers block loading external JSON files due to CORS (Cross-Origin Resource Sharing) security policies.

**Direct File Opening:**
- ❌ Job listings won't load (shows error message)
- ✅ All other features work normally

**Local Server:**
- ✅ Full functionality including dynamic job loading
- ✅ Proper testing environment
- ✅ Matches production behavior

### Alternative Development Options

1. **VS Code Live Server Extension**
   - Install "Live Server" extension
   - Right-click `index-dev.html` → "Open with Live Server"

2. **Other Local Servers**
   ```bash
   # PHP (if available)
   php -S localhost:8000
   
   # Ruby (if available)
   ruby -run -e httpd . -p 8000
   ```

## 📊 Job Listings Management

The development version loads job listings from `jobs.json`. This allows for easy content management without code changes.

### Adding/Editing Jobs

1. **Edit `jobs.json`**
   ```json
   {
     "jobs": [
       {
         "title": "Job Title",
         "location": "Rubixvi • Singapore | Remote",
         "summary": "Brief job description...",
         "description": ["Paragraph 1", "Paragraph 2"],
         "requirements": ["Requirement 1", "Requirement 2"],
         "whoYouAre": ["Trait 1", "Trait 2"],
         "whatYouWillDo": ["Task 1", "Task 2"],
         "contractSetup": ["Detail 1", "Detail 2"]
       }
     ]
   }
   ```

2. **Refresh the page** - Changes appear automatically

### Error Handling

If `jobs.json` fails to load (e.g., CORS issues), the page shows a user-friendly error message instead of breaking.

## 🎨 Styling

- **CSS Framework**: Vanilla CSS with modern features
- **Animations**: anime.js for smooth scroll animations
- **Responsive Design**: Mobile-first approach
- **Color Scheme**: Light backgrounds with brand gradient accents
- **Typography**: Poppins font family

## 🚀 Deployment

The site is automatically deployed via GitHub Pages:

- **Source**: `main` branch, root folder
- **Custom Domain**: www.rubixvi.com (configured via `CNAME`)
- **HTTPS**: Enforced for security
- **Auto-deployment**: Push to main branch triggers deployment

## 🛠️ Technologies Used

- **HTML5**: Semantic markup
- **CSS3**: Modern styling with gradients and animations
- **JavaScript ES6+**: Dynamic content loading and interactions
- **anime.js**: Animation library
- **GitHub Pages**: Hosting and deployment

## 📝 Development Notes

- The development version (`index-dev.html`) is for testing new features
- Production version (`index.html`) should remain stable for the live site
- Job data is separated into JSON for easy content management
- All animations and interactions are progressively enhanced

## 🤝 Contributing

1. Create feature branch from `main`
2. Test changes using local server
3. Update relevant documentation
4. Submit pull request

## 📞 Support

For technical issues or questions:
- **Email**: hello@rubixvi.com
- **GitHub Issues**: Use the repository issue tracker

---

**Note**: This project uses modern web standards. For best experience, use current versions of Chrome, Firefox, Safari, or Edge.