# Portfolio Template 5 - iPortfolio

## Overview

Portfolio Template 5 is based on the **iPortfolio** Bootstrap template. It's a professional, modern portfolio template designed for creative professionals, developers, and designers. The template features a sidebar navigation layout with smooth scrolling and comprehensive sections.

## Features

- **Bootstrap 4**: Built on Bootstrap framework
- **Sidebar Navigation**: Fixed sidebar with profile information
- **Single Page Layout**: All sections on one page with smooth scrolling
- **Portfolio Gallery**: Filterable portfolio with lightbox
- **Resume Section**: Detailed resume/CV display
- **Contact Form**: PHP contact form with email functionality
- **AOS Animations**: Scroll animations for enhanced UX
- **Responsive Design**: Fully responsive mobile-first design
- **Multiple Icon Sets**: Icofont and Boxicons included

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **For contact form**: Ensure PHP is enabled on your server

### Method 2: Local Development Server

1. **Navigate** to the portfolio-5 directory:
   ```bash
   cd portfolio-5
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
portfolio-5/
├── index.html              # Main page (single-page layout)
├── inner-page.html         # Inner page template
├── portfolio-details.html  # Portfolio item detail page
├── assets/
│   ├── css/
│   │   └── style.css      # Main stylesheet
│   ├── img/               # Images
│   │   ├── favicon.png    # Favicon
│   │   ├── profile-img.jpg # Profile image
│   │   └── ... (other images)
│   ├── js/
│   │   └── main.js        # Main JavaScript file
│   └── vendor/            # Third-party libraries
│       ├── bootstrap/     # Bootstrap CSS/JS
│       ├── icofont/       # Icofont icons
│       ├── boxicons/      # Boxicons
│       ├── jquery/        # jQuery library
│       ├── venobox/       # Lightbox plugin
│       ├── owl.carousel/  # Carousel plugin
│       └── aos/           # AOS animation library
├── forms/
│   ├── contact.php        # Contact form handler
│   └── Readme.txt         # Form setup instructions
├── changelog.txt          # Version changelog
└── Readme.txt             # Template information
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Profile Section (Sidebar)
- **File**: `index.html`
- **Location**: Header/Sidebar section (around line 47-50)
- **Update**:
  ```html
  <img src="assets/img/profile-img.jpg" alt="" class="img-fluid rounded-circle">
  <h1 class="text-light"><a href="index.html">Alex Smith</a></h1>
  ```
- **Replace** `profile-img.jpg` with your image
- **Update** name and social links

#### Update About Section
- **File**: `index.html`
- **Find**: `#about` section
- **Update**: Personal information, bio, and details

#### Update Resume Section
- **File**: `index.html`
- **Find**: `#resume` section
- **Update**: Education, professional experience, and skills

### 2. Updating Portfolio Items

1. **File**: `index.html`
2. **Find**: Portfolio section (`#portfolio`)
3. **Structure** for each portfolio item:
   ```html
   <div class="col-lg-4 col-md-6 portfolio-item filter-app">
     <div class="portfolio-wrap">
       <img src="assets/img/portfolio/portfolio-1.jpg" class="img-fluid" alt="">
       <div class="portfolio-links">
         <a href="assets/img/portfolio/portfolio-1.jpg" data-gall="portfolioGallery" class="venobox" title="App 1"><i class="bx bx-plus"></i></a>
         <a href="portfolio-details.html" title="More Details"><i class="bx bx-link"></i></a>
       </div>
     </div>
   </div>
   ```
4. **Filter categories**: `filter-app`, `filter-web`, `filter-card`, etc.
5. **Add images** to `assets/img/portfolio/` folder
6. **Link** to detail pages using `portfolio-details.html` as template

### 3. Updating Skills

1. **File**: `index.html`
2. **Find**: Skills section (`#skills`)
3. **Update** skill items:
   ```html
   <div class="progress">
     <span class="skill">HTML <i class="val">100%</i></span>
     <div class="progress-bar-wrap">
       <div class="progress-bar" role="progressbar" aria-valuenow="100" aria-valuemin="0" aria-valuemax="100"></div>
     </div>
   </div>
   ```
4. **Adjust** skill names and percentages

### 4. Changing Colors

1. **File**: `assets/css/style.css`
2. **Search** for CSS custom properties or color values
3. **Look for** primary color definitions (usually at the top of the file)
4. **Common color variables**:
   ```css
   :root {
     --primary-color: #149ddd;
     --secondary-color: #173b6c;
   }
   ```
5. **Replace** with your brand colors

### 5. Updating Services

1. **File**: `index.html`
2. **Find**: Services section (`#services`)
3. **Update** service items with your offerings
4. **Modify** icons (Icofont or Boxicons classes)

### 6. Customizing Contact Form

1. **File**: `forms/contact.php`
2. **Update** recipient email:
   ```php
   $to = "your-email@example.com";
   ```
3. **Customize** email subject and message format
4. **File**: `index.html` - Update contact form fields as needed

### 7. Changing Profile Image

1. **Replace** `assets/img/profile-img.jpg` with your image
2. **Recommended size**: 400x400px (square, will be displayed as circle)
3. **Format**: JPG or PNG

### 8. Updating Social Links

1. **File**: `index.html`
2. **Find**: Social links in sidebar
3. **Update** URLs:
   ```html
   <a href="https://twitter.com/yourusername" class="twitter"><i class="icofont-twitter"></i></a>
   <a href="https://facebook.com/yourusername" class="facebook"><i class="icofont-facebook"></i></a>
   ```

### 9. Modifying Sidebar

1. **File**: `index.html`
2. **Find**: Sidebar navigation (`.nav-menu`)
3. **Add/Remove** menu items
4. **Update** links to match section IDs

### 10. Creating Portfolio Detail Pages

1. **File**: `portfolio-details.html` (use as template)
2. **Copy** and rename for each portfolio item
3. **Update** content, images, and project details
4. **Link** from portfolio items to detail pages

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
- **Boxicons**: Icon library
- **Venobox**: Lightbox plugin
- **Owl Carousel**: For sliders
- **AOS (Animate On Scroll)**: Scroll animations
- **Google Fonts**: Open Sans, Raleway, Poppins (loaded from CDN)

## Template Information

- **Template Name**: iPortfolio
- **Template URL**: https://bootstrapmade.com/iportfolio-bootstrap-portfolio-websites-template/
- **Author**: BootstrapMade.com
- **License**: Check `Readme.txt` for license information

## Tips

- Test the contact form on a server with PHP enabled
- Optimize images for web (use tools like TinyPNG)
- Keep portfolio images consistent in size for better grid layout
- The sidebar is fixed on desktop, collapses to mobile menu on small screens
- Use AOS data attributes for scroll animations
- Test smooth scrolling navigation on all devices
- Ensure all vendor files are properly linked

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

