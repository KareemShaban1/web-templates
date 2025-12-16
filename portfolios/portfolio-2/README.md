# Portfolio Template 2

## Overview

Portfolio Template 2 is a professional, Bootstrap-based portfolio template with a modern design. It features a single-page layout with smooth scrolling, portfolio filtering, and contact form functionality.

## Features

- **Bootstrap 4**: Built on Bootstrap framework for responsive design
- **Single Page Layout**: All sections on one page with smooth scrolling
- **Portfolio Filtering**: Isotope-based portfolio filter system
- **Contact Form**: PHP contact form with email functionality
- **Multiple Icon Sets**: Icofont, Remixicon, and Boxicons
- **Owl Carousel**: For testimonials and image sliders
- **Venobox**: Lightbox for portfolio images
- **Counter Animation**: Animated statistics counters
- **Responsive Design**: Mobile-first responsive layout

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **For contact form**: Ensure PHP is enabled on your server

### Method 2: Local Development Server

1. **Navigate** to the portfolio-2 directory:
   ```bash
   cd portfolio-2
   ```

2. **Start a local server**:
   - **Python 3**:
     ```bash
     python -m http.server 8000
     ```
   - **Node.js** (with http-server):
     ```bash
     npx http-server -p 8000
     ```
   - **PHP** (recommended for contact form):
     ```bash
     php -S localhost:8000
     ```

3. **Open** your browser and navigate to `http://localhost:8000`

### Contact Form Setup

1. **File**: `forms/contact.php`
2. **Edit** the email configuration:
   ```php
   $to = "your-email@example.com"; // Change to your email
   ```
3. **Ensure** your server supports PHP and mail functionality

## File Structure

```
portfolio-2/
├── index.html              # Main page (single-page layout)
├── portfolio-details.html  # Portfolio item detail page
├── assets/
│   ├── css/
│   │   └── style.css      # Main stylesheet
│   ├── img/               # Images
│   │   ├── bg.jpg         # Background images
│   │   ├── me.jpg         # Profile image
│   │   ├── logo.ico       # Favicon
│   │   ├── portfolio/     # Portfolio images
│   │   └── testimonials/  # Testimonial images
│   ├── js/
│   │   └── main.js        # Main JavaScript file
│   └── vendor/            # Third-party libraries
│       ├── bootstrap/     # Bootstrap CSS/JS
│       ├── icofont/       # Icofont icons
│       ├── remixicon/     # Remixicon icons
│       ├── boxicons/      # Boxicons
│       ├── jquery/        # jQuery library
│       ├── owl.carousel/  # Carousel plugin
│       ├── venobox/       # Lightbox plugin
│       ├── isotope-layout/# Portfolio filter
│       ├── counterup/     # Counter animation
│       └── waypoints/     # Scroll animations
├── forms/
│   ├── contact.php        # Contact form handler
│   └── Readme.txt         # Form setup instructions
└── pages/                 # Additional pages
    ├── frontend/          # Frontend project pages
    ├── laravel/           # Laravel project pages
    └── flutter/           # Flutter project pages
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Header/Name
- **File**: `index.html`
- **Location**: Header section (around line 41):
  ```html
  <h1><a href="index.html">Kareem Shaban</a></h1>
  ```

#### Update About Section
- **File**: `index.html`
- **Find**: `#about` section
- **Update**: Personal information, skills, and experience

#### Update Profile Image
- **File**: `index.html`
- **Location**: About section
- **Replace**: `assets/img/me.jpg` with your image
- **Recommended size**: 400x400px (square)

### 2. Updating Portfolio Items

1. **File**: `index.html`
2. **Find**: Portfolio section (`#portfolio`)
3. **Structure** for each portfolio item:
   ```html
   <div class="col-lg-4 col-md-6 portfolio-item filter-app">
     <div class="portfolio-wrap">
       <img src="assets/img/portfolio/portfolio-1.jpg" class="img-fluid" alt="">
       <div class="portfolio-info">
         <h4>App 1</h4>
         <p>App</p>
       </div>
     </div>
   </div>
   ```
4. **Filter categories**: `filter-app`, `filter-web`, `filter-card`, etc.
5. **Add images** to `assets/img/portfolio/` folder
6. **Create detail pages** in `pages/` folder if needed

### 3. Updating Skills/Resume

1. **File**: `index.html`
2. **Find**: Resume section (`#resume`)
3. **Update**: Education, experience, and skills sections
4. **Skills progress bars**: Adjust percentage values:
   ```html
   <div class="progress-bar" role="progressbar" style="width: 100%" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
   ```

### 4. Changing Colors

1. **File**: `assets/css/style.css`
2. **Search** for color values (hex codes like `#149ddd`)
3. **Replace** with your brand colors
4. **Common color locations**:
   - Primary color: Used for links, buttons, highlights
   - Background colors: Section backgrounds
   - Text colors: Headings and body text

### 5. Updating Testimonials

1. **File**: `index.html`
2. **Find**: Testimonials section
3. **Update**: Testimonial content and images
4. **Add images** to `assets/img/testimonials/` folder

### 6. Customizing Contact Form

1. **File**: `forms/contact.php`
2. **Update** recipient email:
   ```php
   $to = "your-email@example.com";
   ```
3. **Customize** email subject and message format
4. **File**: `index.html` - Update contact form fields as needed

### 7. Changing Background Images

1. **Files**: `assets/img/bg.jpg`, `bg2.jpg`, `bg3.jpg`, `bg4.jpg`
2. **Replace** with your images
3. **Update** references in `index.html` if filenames change
4. **Recommended size**: 1920x1080px

### 8. Adding New Sections

1. **File**: `index.html`
2. **Add** new section with unique ID:
   ```html
   <section id="new-section" class="section">
     <!-- Your content -->
   </section>
   ```
3. **Update** navigation menu to link to new section:
   ```html
   <li><a href="#new-section">New Section</a></li>
   ```

### 9. Modifying Navigation

1. **File**: `index.html`
2. **Find**: Navigation menu (`.nav-menu`)
3. **Add/Remove** menu items
4. **Update** links to match section IDs

### 10. Updating JavaScript

1. **File**: `assets/js/main.js`
2. **Customize** animations, scroll effects, and interactions
3. **Plugin configurations**: Modify settings for carousels, filters, etc.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **Bootstrap 4**: Included in `assets/vendor/bootstrap/`
- **jQuery**: Included in `assets/vendor/jquery/`
- **Icofont**: Icon library
- **Remixicon**: Icon library
- **Boxicons**: Icon library
- **Owl Carousel**: For sliders
- **Venobox**: Lightbox plugin
- **Isotope**: Portfolio filtering
- **CounterUp**: Animated counters
- **Waypoints**: Scroll animations
- **Google Fonts**: Open Sans, Raleway, Poppins (loaded from CDN)

## Tips

- Test the contact form on a server with PHP enabled
- Optimize images for web (use tools like TinyPNG)
- Keep portfolio images consistent in size for better grid layout
- Use the browser developer tools to inspect and modify styles
- Test smooth scrolling navigation on all devices
- Ensure all vendor files are properly linked

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

