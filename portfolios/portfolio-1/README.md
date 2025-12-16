# Portfolio Template 1

## Overview

Portfolio Template 1 is a modern, responsive portfolio website template featuring a unique side navigation design with Material Design icons. It includes multiple color schemes, a preloader, and smooth animations.

## Features

- **Responsive Design**: Fully responsive layout that works on all devices
- **Color Switcher**: 6 different color schemes (Green, Blue, Pink, Orange, Purple, Yellow)
- **Material Design Icons**: Beautiful Material Design icon set
- **Multiple Pages**: Home, About, Services, Portfolio, Blog, and Contact pages
- **Preloader**: Elegant page preloader animation
- **Smooth Animations**: CSS and JavaScript animations for enhanced user experience
- **Blog Articles**: Dedicated articles section with multiple article pages
- **Portfolio Gallery**: Grid-based portfolio showcase with hover effects

## Installation

### Method 1: Direct Use (No Build Process)

1. **Download/Extract** the template files to your web server directory
2. **Open** `index.html` in your browser or upload to a web server
3. **No additional setup required** - all dependencies are included

### Method 2: Local Development Server

1. **Navigate** to the portfolio-1 directory:
   ```bash
   cd portfolio-1
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
portfolio-1/
├── index.html          # Home page
├── about.html          # About page
├── services.html       # Services page
├── portfolio.html      # Portfolio gallery page
├── blog.html           # Blog listing page
├── contact.html        # Contact page
├── Articles/           # Blog article pages
│   ├── article-1.html
│   ├── article-2.html
│   └── ... (article-3 to article-9)
├── CSS/                # Stylesheets
│   ├── bootstrap.min.css
│   ├── style.css       # Main stylesheet
│   ├── type.css        # Typography styles
│   ├── owl.carousel.min.css
│   ├── owl.theme.default.min.css
│   └── color/          # Color scheme files
│       ├── blue.css
│       ├── green.css
│       ├── orange.css
│       ├── pink.css
│       ├── purple.css
│       └── yellow.css
├── JS/                 # JavaScript files
│   ├── jquery-3.5.1.js
│   ├── bootstrap.min.js
│   ├── popper.js
│   ├── script.js       # Main JavaScript file
│   ├── type.js         # Typing animation
│   ├── owl.carousel.min.js
│   ├── masonry.pkgd.min.js
│   └── ... (other plugins)
├── Images/             # Image assets
│   ├── home-bg.jpg
│   ├── project-*.jpg   # Portfolio images
│   ├── blog*.jpg       # Blog images
│   └── testi-*.jpg     # Testimonial images
└── Fonts/              # Font files
    └── MaterialDesign-Webfont-master/
```

## How to Edit the Template

### 1. Changing Personal Information

#### Update Name and Title
- **File**: `index.html` (and other HTML files)
- **Location**: Look for the name in the home section:
  ```html
  <h1>Kareem <span>Shaban</span></h1>
  ```
- **Typing Animation**: Update the typing text in the same file:
  ```html
  <b class="is-visible">Kareem Shaban</b>
  <b>A WEB DESIGNER</b>
  <b>A Backend Developer</b>
  ```

#### Update About Section
- **File**: `about.html`
- Edit the content in the about section to reflect your information

#### Update Contact Information
- **File**: `contact.html`
- Update email, phone, and address information

### 2. Changing Colors

The template includes 6 color schemes. To change the default color:

1. **In `index.html`** (and other HTML files), find this line:
   ```html
   <link rel="stylesheet" type="text/css" href="CSS/color/yellow.css" id="switcher">
   ```

2. **Change** `yellow.css` to your preferred color:
   - `blue.css`
   - `green.css`
   - `orange.css`
   - `pink.css`
   - `purple.css`
   - `yellow.css`

3. **Custom Colors**: To create your own color scheme:
   - Copy one of the color CSS files in `CSS/color/`
   - Rename it (e.g., `custom.css`)
   - Edit the color values in the file
   - Update the link in your HTML files

### 3. Adding/Removing Portfolio Items

1. **File**: `portfolio.html`
2. **Find** the portfolio grid section
3. **Add/Remove** portfolio items by copying the existing structure:
   ```html
   <div class="portfolio-item">
     <img src="Images/project-X.jpg" alt="Project Name">
     <!-- Add project details -->
   </div>
   ```
4. **Add** corresponding images to the `Images/` folder

### 4. Updating Blog Posts

1. **File**: `blog.html` - Update the blog listing
2. **Files**: `Articles/article-*.html` - Edit individual articles
3. **Add new articles** by creating new HTML files in the `Articles/` folder
4. **Update** `blog.html` to link to new articles

### 5. Changing Images

1. **Replace** images in the `Images/` folder
2. **Keep** the same filenames, or update the image paths in HTML files
3. **Recommended sizes**:
   - Portfolio images: 800x600px or similar
   - Blog images: 1200x600px or similar
   - Background images: 1920x1080px or similar

### 6. Customizing Navigation

1. **File**: All HTML files
2. **Find** the navigation sections:
   - Side navigator (`.main-navigator`)
   - Mobile menu (`.mobile-nav`)
3. **Add/Remove** menu items by modifying the navigation lists

### 7. Modifying Styles

1. **Main Styles**: Edit `CSS/style.css`
2. **Color Schemes**: Edit files in `CSS/color/`
3. **Typography**: Edit `CSS/type.css`

### 8. Updating JavaScript Functionality

1. **Main Script**: Edit `JS/script.js`
2. **Typing Animation**: Edit `JS/type.js`
3. **Add custom scripts** in the `JS/` folder and link them in HTML

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Internet Explorer 11+

## Dependencies

- **Bootstrap 4**: Included in `CSS/bootstrap.min.css`
- **jQuery 3.5.1**: Included in `JS/jquery-3.5.1.js`
- **Material Design Icons**: Included in `Fonts/` folder
- **Owl Carousel**: For sliders/carousels
- **Masonry**: For grid layouts
- **Google Fonts**: Poppins and Roboto (loaded from CDN)

## Tips

- Always test changes in multiple browsers
- Keep backup copies before making major changes
- Optimize images before uploading for better performance
- Use the color switcher feature to preview different color schemes
- The template uses relative paths, so it works in subdirectories

## Support

For issues or questions about customization, refer to the main README.md in the portfolios directory.

