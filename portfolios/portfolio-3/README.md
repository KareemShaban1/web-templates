# Portfolio Template 3 - Ronaldo

## Overview

Portfolio Template 3 is the **Ronaldo** Bootstrap 4 template - a modern, single-page portfolio website with smooth scrolling navigation. It features a hero section, comprehensive resume display, portfolio gallery, services section, blog, and contact form. The template includes SCSS source files for easy customization.

## Features

- **Single-Page Layout**: All sections on one page with smooth scrolling
- **Bootstrap 4**: Built on Bootstrap framework for responsive design
- **SCSS Source Files**: Complete SCSS architecture for easy customization
- **Multiple Icon Sets**: Flaticon, Icomoon, and Ionicons included
- **AOS Animations**: Scroll animations for enhanced UX
- **Owl Carousel**: For testimonials and image sliders
- **Magnific Popup**: Lightbox for portfolio images
- **Animated Counters**: Number counting animations
- **Resume Sections**: Education, Experience, Skills, and Awards
- **Responsive Design**: Fully responsive mobile-first design
- **Typing Animation**: Rotating text animation in hero section

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **No additional setup required** - all dependencies are included

### Method 2: Local Development Server

1. **Navigate** to the portfolio-3 directory:
   ```bash
   cd portfolio-3
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

### Method 3: SCSS Development (Optional)

If you want to modify SCSS files:

1. **Use a SCSS compiler** like:
   - Prepros (config file included: `prepros-6.config`)
   - VS Code with Live Sass Compiler extension
   - Command line: `sass scss/style.scss css/style.css --watch`

2. **Edit** files in `scss/` folder
3. **Compile** to `css/style.css`

## File Structure

```
portfolio-3/
├── index.html              # Main page (single-page layout)
├── single.html             # Single blog post template
├── css/                    # Compiled stylesheets
│   ├── style.css          # Main stylesheet
│   ├── bootstrap.min.css  # Bootstrap CSS
│   ├── animate.css        # Animation library
│   ├── aos.css            # AOS animations
│   ├── owl.carousel.min.css # Carousel styles
│   ├── magnific-popup.css # Lightbox styles
│   ├── flaticon.css       # Flaticon icons
│   ├── icomoon.css        # Icomoon icons
│   └── ionicons.min.css   # Ionicons
├── scss/                   # SCSS source files
│   ├── style.scss         # Main SCSS file
│   └── bootstrap/         # Bootstrap SCSS source
├── js/                     # JavaScript files
│   ├── main.js            # Main JavaScript file
│   ├── jquery-3.2.1.min.js # jQuery library
│   ├── bootstrap.min.js   # Bootstrap JS
│   ├── aos.js             # AOS animations
│   ├── owl.carousel.min.js # Carousel plugin
│   ├── jquery.magnific-popup.min.js # Lightbox
│   ├── jquery.animateNumber.min.js # Counter animation
│   ├── jquery.waypoints.min.js # Scroll triggers
│   └── ... (other plugins)
├── images/                 # Image assets
│   ├── about.jpg          # About section image
│   ├── bg_1.jpg, bg_2.png # Background images
│   ├── work-*.jpg         # Portfolio images
│   ├── person_*.jpg       # Team/testimonial images
│   ├── staff-*.jpg        # Staff images
│   └── partner-*.png      # Partner logos
└── fonts/                  # Font files
    ├── flaticon/          # Flaticon font files
    ├── icomoon/           # Icomoon font files
    └── ionicons/          # Ionicons font files
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Hero Section
- **File**: `index.html`
- **Location**: Hero section (around line 54-61)
- **Update**:
  ```html
  <span class="subheading">Hey! I am</span>
  <h1>Ronaldo Fredrickson</h1>
  <h2>I'm a 
    <span class="txt-rotate" data-period="2000"
      data-rotate='[ "Web Designer.", "Developer.", "Photographer.", "Marketer.", "Blogger" ]'></span>
  </h2>
  ```
- **Change** name and rotating text array

#### Update About Section
- **File**: `index.html`
- **Find**: `#about-section` (around line 74)
- **Update**:
  ```html
  <h2 class="mb-4">About Me</h2>
  <p>Your bio text here...</p>
  <ul class="about-info mt-4 px-md-0 px-2">
    <li class="d-flex"><span>Name:</span> <span>Your Name</span></li>
    <li class="d-flex"><span>Date of birth:</span> <span>Your DOB</span></li>
    <li class="d-flex"><span>Address:</span> <span>Your Address</span></li>
    <li class="d-flex"><span>Email:</span> <span>your@email.com</span></li>
    <li class="d-flex"><span>Phone:</span> <span>Your Phone</span></li>
  </ul>
  ```
- **Update** counter number:
  ```html
  <span class="number" data-number="120">0</span>
  <span>Project complete</span>
  ```

#### Update Navigation Brand
- **File**: `index.html`
- **Location**: Navbar (around line 30)
- **Update**:
  ```html
  <a class="navbar-brand" href="index.html"><span>R</span>onaldo</a>
  ```

### 2. Updating Resume Section

#### Education
- **File**: `index.html`
- **Find**: `#page-1` (Education section)
- **Update** each education item:
  ```html
  <div class="resume-wrap d-flex ftco-animate">
    <div class="icon d-flex align-items-center justify-content-center">
      <span class="flaticon-ideas"></span>
    </div>
    <div class="text pl-3">
      <span class="date">2014-2015</span>
      <h2>Degree Name</h2>
      <span class="position">University Name</span>
      <p>Description...</p>
    </div>
  </div>
  ```

#### Experience
- **File**: `index.html`
- **Find**: `#page-2` (Experience section)
- **Update** each experience item (same structure as Education)

#### Skills
- **File**: `index.html`
- **Find**: `#page-3` (Skills section)
- **Update** skill items:
  ```html
  <div class="progress mx-auto" data-value='90'>
    <!-- Progress bar structure -->
    <div class="progress-value w-100 h-100 rounded-circle d-flex align-items-center justify-content-center">
      <div class="h2 font-weight-bold">90<sup class="small">%</sup></div>
    </div>
  </div>
  ```
- **Change** `data-value` and percentage display

#### Awards
- **File**: `index.html`
- **Find**: `#page-4` (Awards section)
- **Update** award items

### 3. Updating Portfolio/Projects

1. **File**: `index.html`
2. **Find**: `#projects-section` (around line 566)
3. **Structure** for each project:
   ```html
   <div class="col-md-4">
     <div class="project img ftco-animate d-flex justify-content-center align-items-center" style="background-image: url(images/work-1.jpg);">
       <div class="overlay"></div>
       <div class="text text-center p-4">
         <h3><a href="project.html">Project Name</a></h3>
         <span>Category</span>
       </div>
     </div>
   </div>
   ```
4. **Add images** to `images/` folder
5. **Update** background-image URLs

### 4. Updating Services

1. **File**: `index.html`
2. **Find**: `#services-section` (around line 484)
3. **Update** service items with your offerings
4. **Modify** icons (Flaticon classes)

### 5. Changing Colors

#### Method 1: Edit SCSS (Recommended)
1. **File**: `scss/style.scss`
2. **Find** color variables (usually at the top)
3. **Update** primary, secondary, and accent colors
4. **Compile** SCSS to CSS

#### Method 2: Edit Compiled CSS
1. **File**: `css/style.css`
2. **Search** for color values (hex codes)
3. **Replace** with your brand colors
4. **Common locations**:
   - Primary color: Buttons, links, highlights
   - Background colors: Section backgrounds
   - Text colors: Headings and body text

### 6. Updating Blog Section

1. **File**: `index.html`
2. **Find**: `#blog-section` (around line 675)
3. **Update** blog post items
4. **Link** to `single.html` for individual posts
5. **Customize** `single.html` for blog post layout

### 7. Customizing Contact Form

1. **File**: `index.html`
2. **Find**: `#contact-section` (around line 753)
3. **Update** contact form fields
4. **Configure** form action (may need PHP backend)
5. **Update** contact information display

### 8. Changing Images

1. **Replace** images in `images/` folder
2. **Keep** the same filenames, or update image paths in HTML
3. **Recommended sizes**:
   - About image: 800x1000px or similar
   - Portfolio images: 800x600px or similar
   - Background images: 1920x1080px or similar
   - Profile/team images: 400x400px (square)

### 9. Modifying Navigation

1. **File**: `index.html`
2. **Find**: Navigation menu (around line 36-44)
3. **Add/Remove** menu items:
   ```html
   <li class="nav-item"><a href="#section-id" class="nav-link"><span>Section Name</span></a></li>
   ```
4. **Update** links to match section IDs

### 10. Updating Typing Animation

1. **File**: `index.html`
2. **Find**: Hero section typing animation
3. **Update** the data-rotate array:
   ```html
   data-rotate='[ "Text 1.", "Text 2.", "Text 3." ]'
   ```

### 11. Customizing Icons

The template uses multiple icon sets:
- **Flaticon**: Use classes like `flaticon-ideas`
- **Icomoon**: Use classes like `icon-*`
- **Ionicons**: Use classes like `ion-*`

1. **Browse** available icons in the font files
2. **Replace** icon classes in HTML
3. **Ensure** corresponding font files are included

### 12. Modifying SCSS Styles

1. **File**: `scss/style.scss`
2. **Edit** styles as needed
3. **Compile** to CSS:
   ```bash
   sass scss/style.scss css/style.css
   ```
4. **Or use** Prepros with the included config file

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **Bootstrap 4**: Included in `css/bootstrap.min.css`
- **jQuery 3.2.1**: Included in `js/jquery-3.2.1.min.js`
- **AOS (Animate On Scroll)**: For scroll animations
- **Owl Carousel**: For sliders/carousels
- **Magnific Popup**: For lightbox galleries
- **Waypoints**: For scroll triggers
- **AnimateNumber**: For counter animations
- **Flaticon**: Icon library
- **Icomoon**: Icon library
- **Ionicons**: Icon library
- **Google Fonts**: Poppins (loaded from CDN)

## Template Information

- **Template Name**: Ronaldo
- **Source**: Colorlib Free Bootstrap 4 Template
- **Framework**: Bootstrap 4
- **Layout**: Single-page

## Tips

- Use the SCSS files for easier color and style customization
- Test smooth scrolling navigation on all devices
- Optimize images before uploading for better performance
- Keep portfolio images consistent in size for better grid layout
- Use browser developer tools to inspect and modify styles
- The template uses data attributes for animations (data-number, data-rotate, etc.)
- Ensure all font files are properly linked for icons to display
- Test all sections on mobile devices for responsiveness

## Common Customization Tasks

### Change Primary Color
1. Edit `scss/style.scss` or `css/style.css`
2. Search for primary color values
3. Replace with your brand color

### Add New Section
1. Add new section with unique ID in `index.html`
2. Update navigation menu
3. Style in SCSS/CSS

### Modify Typography
1. Edit font imports in HTML head
2. Update font-family in SCSS/CSS
3. Adjust font sizes and weights

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.
