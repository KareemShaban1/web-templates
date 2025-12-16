# Portfolio Template 4 - Epitome

## Overview

Portfolio Template 4 is the **Epitome** free resume and personal portfolio website template. It's a modern, trendy template with a visually attractive design, ideal for creative professionals and freelancers. The template features a fullscreen hero banner, about section, services, portfolio, testimonials, and contact section.

## Features

- **Single-Page Layout**: All sections on one page with smooth scrolling
- **Fullscreen Hero Banner**: Eye-catching hero section
- **Modern Design**: Clean and trendy aesthetic
- **Mobile & Retina Ready**: Looks great on all devices and screen resolutions
- **Portfolio Gallery**: Masonry grid layout for projects
- **Testimonials Section**: Client testimonials display
- **Work & Education Timeline**: Visual timeline for experience
- **AOS Animations**: Scroll animations for enhanced UX
- **Preloader**: Page loading animation
- **Responsive Design**: Fully responsive mobile-first design

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **No additional setup required** - all dependencies are included

### Method 2: Local Development Server

1. **Navigate** to the portfolio-4 directory:
   ```bash
   cd portfolio-4
   ```

2. **Start a local server** (choose one):
   - **Python 3**:
     ```bash
     python -m http.server 8000
     ```
   - **Node.js** (with http-server):
     ```bash
     npx http-server -p 8000
     ```
   - **PHP**:
     ```bash
     php -S localhost:8000
     ```

3. **Open** your browser and navigate to `http://localhost:8000`

## File Structure

```
portfolio-4/
├── index.html              # Main page (single-page layout)
├── styles.html             # Styles showcase page
├── css/                    # Stylesheets
│   ├── base.css           # Base styles
│   ├── main.css           # Main stylesheet
│   ├── vendor.css         # Vendor styles
│   └── font-awesome/      # Font Awesome icons
├── js/                     # JavaScript files
│   ├── main.js            # Main JavaScript file
│   ├── jquery-3.2.1.min.js # jQuery library
│   ├── modernizr.js       # Modernizr
│   ├── pace.min.js        # Preloader
│   └── plugins.js         # Plugin initialization
├── images/                 # Image assets
│   ├── logo.svg           # Site logo
│   └── ... (other images)
├── favicon.ico            # Favicon
├── apple-touch-icon.png   # Apple touch icon
├── site.webmanifest       # Web manifest
└── readme.txt             # Template information
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Intro/Hero Section
- **File**: `index.html`
- **Location**: Intro section (`#intro`, around line 76-100)
- **Update**:
  ```html
  <h3>Hello, I'm John Doe</h3>
  <h1>
    Digital Designer <br>
    and Web Developer <br>
    Based In Somewhere.
  </h1>
  ```

#### Update About Section
- **File**: `index.html`
- **Find**: `#about` section (around line 105)
- **Update**:
  ```html
  <h2 class="section-heading">About Me</h2>
  <p class="lead">Your bio text here...</p>
  ```
- **Update** personal information and bio

#### Update Logo
- **File**: `index.html`
- **Location**: Header (around line 47-48)
- **Replace**: `images/logo.svg` with your logo
- **Or** update the logo image path

### 2. Updating Work & Education Timeline

1. **File**: `index.html`
2. **Find**: Work & Education section (around line 163)
3. **Structure** for timeline items:
   ```html
   <div class="timeline__block">
     <div class="timeline__bullet"></div>
     <div class="timeline__header">
       <p class="timeline__timeframe">July 2018 - Present</p>
       <h3 class="item-title">Company Name</h3>
       <h5>Job Title</h5>
     </div>
     <div class="timeline__desc">
       <p>Job description...</p>
     </div>
   </div>
   ```
4. **Add/Remove** timeline blocks for work experience
5. **Education** follows the same structure

### 3. Updating Services/Capabilities

1. **File**: `index.html`
2. **Find**: Services section (`#services`, around line 273)
3. **Update** service items:
   ```html
   <div class="item-folio">
     <div class="item-folio__thumb">
       <a href="images/portfolio/gallery/g-*.jpg" class="thumb-link" title="Service Name" data-size="1050x700">
         <img src="images/portfolio/thumb.jpg" alt="">
       </a>
     </div>
     <div class="item-folio__text">
       <h3 class="item-folio__title">Service Name</h3>
       <p class="item-folio__cat">Category</p>
     </div>
   </div>
   ```

### 4. Updating Portfolio/Works

1. **File**: `index.html`
2. **Find**: Works section (`#works`, around line 389)
3. **Structure** for portfolio items:
   ```html
   <div class="masonry__brick">
     <div class="item-folio">
       <div class="item-folio__thumb">
         <a href="images/portfolio/gallery/g-*.jpg" class="thumb-link" data-size="1050x700">
           <img src="images/portfolio/thumb.jpg" alt="">
         </a>
       </div>
       <div class="item-folio__text">
         <h3 class="item-folio__title">Project Title</h3>
         <p class="item-folio__cat">Category</p>
       </div>
     </div>
   </div>
   ```
4. **Add images** to `images/portfolio/` folder
5. **Masonry** layout will automatically arrange items

### 5. Updating Testimonials

1. **File**: `index.html`
2. **Find**: Testimonials section
3. **Update** testimonial items with client feedback
4. **Add** client images if needed

### 6. Changing Colors

1. **File**: `css/main.css`
2. **Search** for color values (hex codes)
3. **Replace** with your brand colors
4. **Common color locations**:
   - Primary color: Links, buttons, highlights
   - Background colors: Section backgrounds
   - Text colors: Headings and body text
   - Accent colors: Hover states, borders

### 7. Customizing Contact Section

1. **File**: `index.html`
2. **Find**: Contact section (`#contact`)
3. **Update** contact form fields
4. **Update** contact information display
5. **Configure** form action (may need PHP backend)

### 8. Changing Images

1. **Replace** images in `images/` folder
2. **Keep** the same filenames, or update image paths in HTML
3. **Recommended sizes**:
   - Portfolio images: 1050x700px or similar
   - Hero background: 1920x1080px or similar
   - Profile images: 400x400px (square)
   - Logo: SVG format preferred

### 9. Modifying Navigation

1. **File**: `index.html`
2. **Find**: Header navigation (around line 52-59)
3. **Add/Remove** menu items:
   ```html
   <li><a class="smoothscroll" href="#section-id" title="Section Name">Section Name</a></li>
   ```
4. **Update** links to match section IDs

### 10. Updating Social Links

1. **File**: `index.html`
2. **Find**: Social links in header (around line 61-66)
3. **Update** URLs:
   ```html
   <li><a href="https://twitter.com/yourusername"><i class="fab fa-twitter" aria-hidden="true"></i></a></li>
   <li><a href="https://facebook.com/yourusername"><i class="fab fa-facebook-f" aria-hidden="true"></i></a></li>
   ```

### 11. Modifying Styles

1. **Main Styles**: Edit `css/main.css`
2. **Base Styles**: Edit `css/base.css`
3. **Vendor Styles**: Edit `css/vendor.css` (if needed)
4. **Use** browser developer tools to inspect and modify styles

### 12. Updating JavaScript

1. **File**: `js/main.js`
2. **Customize** animations, scroll effects, and interactions
3. **Plugin settings**: Modify Masonry, AOS, and other plugin configurations

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **jQuery 3.2.1**: Included in `js/jquery-3.2.1.min.js`
- **Modernizr**: Feature detection library
- **Masonry JS**: For portfolio grid layout
- **ImagesLoaded**: For image loading detection
- **Slick Slider**: For carousels/sliders
- **AOS (Animate On Scroll)**: Scroll animations
- **Pace JS**: Preloader animation
- **Font Awesome**: Icon library
- **Google Fonts**: Lora, Roboto, Frank Ruhl Libre (loaded from CDN)

## Template Information

- **Template Name**: Epitome
- **Source**: Styleshout.com
- **License**: Free for personal and commercial use (with attribution)
- **Attribution**: Credit link to styleshout.com required

## Credits

- **Fonts**: Lora, Roboto, Frank Ruhl Libre (Google Fonts)
- **Icons**: Font Awesome, Iconmonstr
- **Stock Photos**: Unsplash.com
- **JavaScript Libraries**: jQuery, Modernizr, Masonry, ImagesLoaded, Slick, AOS, Pace

## Tips

- Test smooth scrolling navigation on all devices
- Optimize images for web (use tools like TinyPNG)
- Keep portfolio images consistent in aspect ratio for better grid layout
- Use the preloader to enhance perceived performance
- The template uses Masonry for automatic grid arrangement
- Test all sections on mobile devices for responsiveness
- Use browser developer tools to inspect and modify styles
- SVG format is preferred for logos and icons

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

**Note**: This template requires attribution to styleshout.com. See `readme.txt` for license details.
