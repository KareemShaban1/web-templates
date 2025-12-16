# Portfolio Template 6 - JohnDoe

## Overview

Portfolio Template 6 is the **JohnDoe** Bootstrap landing page template. It's an elegant, responsive Bootstrap 4.x theme designed for personal portfolios and professional websites. The template includes a build system using Gulp for development and optimization.

## Features

- **Bootstrap 4**: Built on Bootstrap 4 framework
- **Gulp Build System**: Automated build process for development
- **SCSS/SASS**: Modular SCSS architecture for easy customization
- **Responsive Design**: Mobile-first responsive layout
- **Smooth Scrolling**: One-page layout with smooth scroll navigation
- **Component Library**: Dedicated components page for easy reference
- **Modern Design**: Clean and modern aesthetic
- **Themify Icons**: Beautiful icon set included

## Installation

### Method 1: Direct Use (No Build Process)

1. **Navigate** to the `public_html` directory:
   ```bash
   cd portfolio-6/public_html
   ```

2. **Open** `index.html` in your browser or upload to a web server
3. **No build process required** - compiled files are included

### Method 2: Development with Gulp (Recommended)

1. **Prerequisites**: Install Node.js and npm

2. **Navigate** to the portfolio-6 directory:
   ```bash
   cd portfolio-6
   ```

3. **Install dependencies**:
   ```bash
   npm install
   ```

4. **Start development server**:
   ```bash
   npm start
   ```
   This will:
   - Start a local server (usually at `http://localhost:3000`)
   - Watch for file changes
   - Auto-reload the browser
   - Compile SCSS to CSS
   - Process and optimize assets

5. **Build for production**:
   ```bash
   gulp build
   ```

### Method 3: Simple Local Server

1. **Navigate** to the `public_html` directory:
   ```bash
   cd portfolio-6/public_html
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

3. **Open** your browser and navigate to `http://localhost:8000`

## File Structure

```
portfolio-6/
├── public_html/          # Main website files
│   ├── index.html       # Home page
│   ├── components.html  # Components showcase page
│   └── assets/
│       ├── css/
│       │   └── johndoe.css  # Compiled CSS
│       ├── js/
│       │   └── johndoe.js   # JavaScript files
│       ├── imgs/        # Images
│       └── vendors/     # Third-party libraries
│           ├── bootstrap/   # Bootstrap files
│           ├── themify-icons/ # Icon library
│           └── ... (other vendors)
├── gulpfile.js          # Gulp configuration
├── package.json         # Node.js dependencies
└── README.txt           # Template information
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Header Section
- **File**: `public_html/index.html`
- **Location**: Header section (around line 26-28)
- **Update**:
  ```html
  <h4 class="header-subtitle">Hello, I am</h4>
  <h1 class="header-title">John Doe</h1>
  <h6 class="header-mono">Front end Designer | Developer</h6>
  ```

#### Update About Section
- **File**: `public_html/index.html`
- **Find**: About section (`#about`)
- **Update**: Personal information, bio, and details

#### Update Resume Section
- **File**: `public_html/index.html`
- **Find**: Resume section (`#resume`)
- **Update**: Education, experience, and skills

### 2. Updating Portfolio Items

1. **File**: `public_html/index.html`
2. **Find**: Portfolio section
3. **Structure** for each portfolio item:
   ```html
   <div class="col-md-4">
     <a href="assets/imgs/folio-1.jpg" class="portfolio-card">
       <img src="assets/imgs/folio-1.jpg" class="portfolio-card-img" alt="">
       <span class="portfolio-card-overlay">
         <span class="portfolio-card-caption">
           <h4>Project Title</h4>
           <p class="font-weight-normal">Category</p>
         </span>
       </span>
     </a>
   </div>
   ```
4. **Add images** to `public_html/assets/imgs/` folder
5. **Update** project titles and categories

### 3. Changing Colors

#### Method 1: Edit SCSS (If using Gulp)
1. **File**: SCSS source files (if available)
2. **Find** color variables
3. **Update** primary, secondary, and accent colors
4. **Run** `gulp` to recompile

#### Method 2: Edit Compiled CSS
1. **File**: `public_html/assets/css/johndoe.css`
2. **Search** for color values (hex codes)
3. **Replace** with your brand colors
4. **Common locations**:
   - Primary color: Buttons, links, highlights
   - Background colors: Section backgrounds
   - Text colors: Headings and body text

### 4. Updating Skills

1. **File**: `public_html/index.html`
2. **Find**: Skills section
3. **Update** skill items with your skills and proficiency levels

### 5. Customizing Navigation

1. **File**: `public_html/index.html`
2. **Find**: Navigation menu (`.navbar`)
3. **Add/Remove** menu items:
   ```html
   <li class="nav-item">
     <a href="#section-id" class="nav-link">Section Name</a>
   </li>
   ```
4. **Update** links to match section IDs

### 6. Updating Social Links

1. **File**: `public_html/index.html`
2. **Find**: Social icons in header (around line 18-23)
3. **Update** URLs:
   ```html
   <li class="social-item">
     <a class="social-link text-light" href="https://twitter.com/yourusername">
       <i class="ti-twitter"></i>
     </a>
   </li>
   ```

### 7. Changing Images

1. **Replace** images in `public_html/assets/imgs/` folder
2. **Keep** the same filenames, or update image paths in HTML
3. **Recommended sizes**:
   - Portfolio images: 800x600px or similar
   - Header background: 1920x1080px or similar
   - Profile images: 400x400px or similar

### 8. Adding New Sections

1. **File**: `public_html/index.html`
2. **Add** new section with unique ID:
   ```html
   <section id="new-section" class="section">
     <div class="container">
       <!-- Your content -->
     </div>
   </section>
   ```
3. **Update** navigation menu to link to new section

### 9. Modifying Styles (Development Mode)

If using Gulp for development:

1. **Edit** SCSS source files
2. **Gulp** will automatically:
   - Compile SCSS to CSS
   - Auto-prefix CSS
   - Minify CSS
   - Reload browser

3. **For production**:
   ```bash
   gulp build
   ```

### 10. Updating JavaScript

1. **File**: `public_html/assets/js/johndoe.js` (or separate JS files)
2. **Customize** animations, scroll effects, and interactions
3. **If using Gulp**: Edit source JS files, Gulp will process them

## Gulp Tasks

If using the Gulp build system:

- **`npm start`** or **`gulp`**: Start development server with watch
- **`gulp build`**: Build for production (minify, optimize)
- **`gulp clean`**: Clean build directories
- **`gulp images`**: Optimize images

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **Bootstrap 4**: Included in `public_html/assets/vendors/bootstrap/`
- **jQuery**: Included via CDN or vendor files
- **Themify Icons**: Icon library
- **Isotope**: For portfolio filtering (if used)
- **Google Maps**: For contact map (if used)

## Template Information

- **Template Name**: JohnDoe
- **Version**: 1.5.0
- **Author**: DevCRUD
- **Product Page**: https://www.devcrud.com/
- **License**: Check `README.txt` for license information

## Credits

- **Demo Images**: Unsplash (https://www.unsplash.com)
- **Icons**: Themify Icons (https://themify.me/themify-icons)
- **jQuery**: https://www.jquery.com
- **Bootstrap**: https://www.getbootstrap.com

## Tips

- Use the components page (`components.html`) as a reference for available components
- If using Gulp, keep the development server running while making changes
- Optimize images before uploading for better performance
- Test smooth scrolling navigation on all devices
- The template uses Bootstrap's affix for sticky navigation
- Use browser developer tools to inspect and modify styles
- For production, always run `gulp build` to optimize assets

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

