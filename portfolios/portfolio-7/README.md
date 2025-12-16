# Portfolio Template 7 - Marvel

## Overview

Portfolio Template 7 is the **Marvel** HTML Bootstrap 4 template from Tooplate. It's a modern, responsive portfolio template designed for personal portfolios and professional websites. The template features a clean design with animated text, color mode toggle, and smooth scrolling navigation.

## Features

- **Bootstrap 4**: Built on Bootstrap 4 framework
- **Single-Page Layout**: All sections on one page with smooth scrolling
- **Animated Text**: Typing animation effect in hero section
- **Color Mode Toggle**: Dark/light mode switcher
- **Responsive Design**: Mobile-first responsive layout
- **Modern UI**: Clean and modern aesthetic
- **Unicons**: Beautiful icon set included
- **Owl Carousel**: For project sliders
- **Smooth Animations**: CSS and JavaScript animations

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **No additional setup required** - all dependencies are included

### Method 2: Local Development Server

1. **Navigate** to the portfolio-7 directory:
   ```bash
   cd portfolio-7
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
portfolio-7/
├── index.html              # Main page (single-page layout)
├── css/                    # Stylesheets
│   ├── bootstrap.min.css  # Bootstrap CSS
│   ├── unicons.css        # Unicons icon library
│   ├── owl.carousel.min.css # Carousel styles
│   ├── owl.theme.default.min.css
│   └── tooplate-style.css # Main stylesheet
├── js/                     # JavaScript files
│   ├── jquery.min.js      # jQuery library
│   ├── bootstrap.min.js   # Bootstrap JS
│   ├── owl.carousel.min.js # Carousel plugin
│   └── main.js            # Main JavaScript file
├── images/                 # Image assets
│   ├── project/           # Project images
│   └── undraw/            # SVG illustrations
├── font/                   # Font files
│   └── ... (font files)
├── sass/                   # SASS source files (optional)
│   └── tooplate-style.scss
└── ABOUT THIS TEMPLATE.txt # Template information
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Hero/About Section
- **File**: `index.html`
- **Location**: About section (`#about`, around line 70-92)
- **Update**:
  ```html
  <small class="small-text">Welcome to <span class="mobile-block">my portfolio website!</span></small>
  <h1 class="animated animated-text">
    <span class="mr-2">Hey folks, I'm</span>
    <div class="animated-info">
      <span class="animated-item">Marvel Sann</span>
      <span class="animated-item">Web Designer</span>
      <span class="animated-item">UI Specialist</span>
    </div>
  </h1>
  <p>Your bio text here...</p>
  ```
- **Change** name, animated text items, and bio

#### Update Navigation Brand
- **File**: `index.html`
- **Location**: Navbar (around line 32)
- **Update**:
  ```html
  <a class="navbar-brand" href="index.html"><i class='uil uil-user'></i> Marvel</a>
  ```

### 2. Updating Projects

1. **File**: `index.html`
2. **Find**: Project section (`#project`)
3. **Structure** for each project:
   ```html
   <div class="col-lg-4 col-md-6">
     <div class="project-info">
       <img src="images/project/project-image.png" class="img-fluid" alt="project image">
       <div class="project-info-content">
         <h4 class="text-white">Project Title</h4>
         <p class="text-white">Project Description</p>
       </div>
     </div>
   </div>
   ```
4. **Add images** to `images/project/` folder
5. **Update** project titles and descriptions

### 3. Updating Resume Section

1. **File**: `index.html`
2. **Find**: Resume section (`#resume`)
3. **Update** education, experience, and skills
4. **Structure** for resume items:
   ```html
   <div class="resume-item">
     <h5>Job Title / Degree</h5>
     <p><strong>Company / Institution</strong> - Year</p>
     <p>Description...</p>
   </div>
   ```

### 4. Changing Colors

1. **File**: `css/tooplate-style.css`
2. **Search** for color values (hex codes)
3. **Replace** with your brand colors
4. **Common color locations**:
   - Primary color: Buttons, links, highlights
   - Background colors: Section backgrounds
   - Text colors: Headings and body text
5. **Color Mode**: The template includes dark/light mode toggle functionality

### 5. Customizing Color Mode

1. **File**: `js/main.js`
2. **Find** color mode toggle functionality
3. **Customize** color schemes for light and dark modes
4. **Update** CSS variables or classes for each mode

### 6. Updating Animated Text

1. **File**: `index.html`
2. **Find**: Animated text section
3. **Update** the animated items:
   ```html
   <div class="animated-info">
     <span class="animated-item">Text 1</span>
     <span class="animated-item">Text 2</span>
     <span class="animated-item">Text 3</span>
   </div>
   ```

### 7. Customizing Navigation

1. **File**: `index.html`
2. **Find**: Navigation menu (around line 42-55)
3. **Add/Remove** menu items:
   ```html
   <li class="nav-item">
     <a href="#section-id" class="nav-link"><span data-hover="Section Name">Section Name</span></a>
   </li>
   ```
4. **Update** links to match section IDs

### 8. Updating Social Links

1. **File**: `index.html`
2. **Find**: Social links section (if present)
3. **Update** URLs and icon classes (Unicons)

### 9. Changing Images

1. **Replace** images in `images/` folder
2. **Keep** the same filenames, or update image paths in HTML
3. **Recommended sizes**:
   - Project images: 800x600px or similar
   - Profile images: 400x400px (square)
   - SVG illustrations: Use from `images/undraw/` or add your own

### 10. Modifying Styles

#### Method 1: Edit CSS
1. **File**: `css/tooplate-style.css`
2. **Edit** styles as needed
3. **Test** changes in browser

#### Method 2: Edit SASS (If Available)
1. **File**: `sass/tooplate-style.scss`
2. **Edit** SASS variables and styles
3. **Compile** to CSS:
   ```bash
   sass sass/tooplate-style.scss css/tooplate-style.css
   ```

### 11. Updating JavaScript

1. **File**: `js/main.js`
2. **Customize** animations, scroll effects, and interactions
3. **Color mode toggle**: Modify dark/light mode functionality
4. **Animated text**: Adjust animation timing and effects

### 12. Adding New Sections

1. **File**: `index.html`
2. **Add** new section with unique ID:
   ```html
   <section id="new-section" class="section">
     <div class="container">
       <!-- Your content -->
     </div>
   </section>
   ```
3. **Update** navigation menu to link to new section

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **Bootstrap 4**: Included in `css/bootstrap.min.css`
- **jQuery**: Included in `js/jquery.min.js`
- **Unicons**: Icon library (included in `css/unicons.css`)
- **Owl Carousel**: For sliders/carousels
- **Google Fonts**: Various fonts (loaded from CDN if used)

## Template Information

- **Template Name**: Marvel
- **Template Number**: Tooplate 2115
- **Source**: Tooplate.com
- **License**: Free to use for personal and commercial projects
- **Restrictions**: Cannot redistribute template files on template sites

## Credits

- **Template**: Tooplate.com
- **Icons**: Unicons
- **Framework**: Bootstrap 4

## Tips

- Use the color mode toggle to test both light and dark themes
- Optimize images for web (use tools like TinyPNG)
- Keep project images consistent in size for better grid layout
- Test animated text on different devices
- Use browser developer tools to inspect and modify styles
- The template uses smooth scrolling for navigation
- SVG illustrations can be customized or replaced
- Test all sections on mobile devices for responsiveness

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

**Note**: See `ABOUT THIS TEMPLATE.txt` for license and usage information.

