# Allied Agencies Cochin - Water Pump Solutions

A modern, responsive website for Allied Agencies Cochin, established in 1973, specializing in premium water pump solutions for residential, industrial, and agricultural applications.

## 🚀 Features

- **Modern Design**: Clean, professional interface with smooth animations
- **Responsive**: Works perfectly on all devices (mobile, tablet, desktop)
- **Content Management**: Built-in admin panel for easy content updates
- **SEO Optimized**: Proper meta tags, sitemap, and robots.txt
- **Performance**: Optimized for fast loading and excellent user experience
- **Security**: Security headers and best practices implemented

## 📁 Project Structure

```
allied-agencies-cochin/
├── index.html              # Main website (1,200+ lines)
├── admin.html              # Content management panel (1,000+ lines)
├── README.md               # This file
└── src/                    # Source data files
    └── data/               # JSON data files
        ├── products.json   # Product catalog (6 products)
        ├── brands.json     # Partner brands (5 brands)
        └── contact.json    # Contact information
```

## 🎯 Technologies

- **Pure HTML/CSS/JavaScript**: No frameworks, dependencies, or build tools required
- **CSS Grid & Flexbox**: Modern layout techniques for responsive design
- **CSS Variables**: Easy theming and customization without code changes
- **Intersection Observer API**: Smooth scroll animations and reveal effects
- **Local Storage API**: Client-side data persistence for content management
- **Mobile-First Responsive Design**: Works perfectly on all screen sizes
- **Google Fonts**: Professional typography with web-safe fallbacks
- **Unsplash Images**: High-quality placeholder images (replaceable with real product photos)

## 📊 Data Management

### Products (6 items in catalog)
- Name, category, description, image URL
- Status (available/unavailable) 
- Featured flag for highlighting
- Categories: Residential, Industrial, Agriculture, Renewable, Commercial, Treatment
- Each product has unique ID for management

### Brands (5 partner brands)
- Name, logo URL, description
- Website URL for external links
- Featured flag for highlighting
- Partner logos with hover effects and grayscale transitions
- Real brands: Kirloskar, V-Guard, Texmo, CRI Pumps, Lubi

### Contact Information
- Phone number with WhatsApp integration
- Email address for inquiries
- Physical address with line breaks
- Business hours and operating days
- Google Maps embed URL for location
- Social media links (Facebook, Instagram, LinkedIn)

## 🛠️ Development

### Local Development
1. Open `index.html` directly in any modern browser (Chrome, Firefox, Safari, Edge)
2. For content management, open `admin.html` in a separate tab
3. No build tools, dependencies, or local server required
4. Changes are saved automatically to browser LocalStorage

### Testing the Website

#### Basic Functionality Testing
1. **Navigation**: Test all menu links (Home, About, Brands, Products, Contact)
2. **Mobile Responsiveness**: Resize browser window or use device emulation
3. **Product Gallery**: Test category filters and product cards
4. **Contact Links**: Verify WhatsApp and email links work
5. **Scroll Animations**: Check smooth scrolling and reveal effects

#### Admin Panel Testing
1. **Product Management**: 
   - Add a new product with all fields filled
   - Edit existing products
   - Delete test products
   - Test image upload (drag & drop or click to upload)
   - Verify changes appear instantly on main website

2. **Brand Management**:
   - Add/edit/delete brands
   - Test logo upload functionality
   - Verify brand marquee updates

3. **Contact Management**:
   - Update phone, email, address
   - Test Google Maps embed URL
   - Verify contact information updates on main site

4. **Data Operations**:
   - Export data and verify JSON structure
   - Import data and confirm restoration
   - Test clear storage functionality

#### Cross-Browser Testing
- **Chrome/Edge**: Full feature support
- **Firefox**: All features supported
- **Safari**: All features supported
- **Mobile browsers**: Responsive design should work on iOS/Android

#### Performance Testing
1. **Page Load Speed**: Check loading times for main page
2. **Image Loading**: Verify lazy loading works correctly
3. **LocalStorage**: Confirm data persists between browser sessions
4. **Memory Usage**: Monitor for any memory leaks during extended admin use

### Content Management
1. Open `admin.html` in your browser
2. Use the admin panel to:
   - Add/edit/delete products
   - Manage partner brands
   - Update contact information
   - Export/import data
   - Clear local storage

### Data Structure

#### Products JSON
```json
{
  "id": "unique-id",
  "name": "Product Name",
  "category": "Category Name",
  "description": "Product description",
  "image": "image-url.jpg",
  "featured": true/false,
  "status": "available/unavailable"
}
```

#### Brands JSON
```json
{
  "id": "unique-id", 
  "name": "Brand Name",
  "logo": "logo-url.png",
  "description": "Brand description",
  "website": "website-url.com",
  "featured": true/false
}
```

#### Contact JSON
```json
{
  "whatsappNumber": "919846012345",
  "displayPhone": "+91 98460 12345",
  "email": "sales@alliedcochin.com",
  "address": "Full address",
  "hours": "10:00 AM – 7:00 PM",
  "days": "Mon — Sat",
  "mapEmbedUrl": "Google Maps embed URL",
  "social": {
    "facebook": "Facebook URL",
    "instagram": "Instagram URL", 
    "linkedin": "LinkedIn URL"
  }
}
```

## 🚀 Deployment

### Local Development
1. Open `index.html` directly in any modern browser
2. No server or build process required
3. For content management, open `admin.html`

### GitHub Pages
1. **Create GitHub Repository**: Push your project files to a new GitHub repository
2. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Source", select "Deploy from a branch"
   - Choose the `main` branch (or your default branch)
   - Click "Save"
3. **Wait for Deployment**: GitHub will deploy your site (usually takes 1-5 minutes)
4. **Access Your Site**: Your website will be available at `https://yourusername.github.io/repository-name`

**Important Notes**:
- No build process required - GitHub Pages serves static HTML files directly
- Both `index.html` and `admin.html` will be accessible
- The admin panel will work with browser LocalStorage
- Ensure your repository is public for free GitHub Pages hosting

### Netlify
1. Connect GitHub repository
2. No build command needed (static site)
3. Set publish directory: `.` (root)
4. Deploy

### Vercel
1. Import GitHub repository
2. No build command needed (static site)
3. Set output directory: `.` (root)
4. Deploy

### Apache/Nginx
1. Upload project files to web server
2. Configure web server to serve static files
3. Set `index.html` as default document

## 🚀 Features (Updated)

- **Modern Design**: Clean, professional interface with smooth animations using CSS Grid/Flexbox
- **Responsive**: Mobile-first design that works perfectly on all devices
- **Content Management**: Built-in admin panel (`admin.html`) for easy content updates without coding
- **SEO Optimized**: Proper meta tags, Open Graph tags, and semantic HTML structure
- **Performance**: Optimized images, lazy loading, and efficient CSS/JS
- **Data Persistence**: LocalStorage for client-side data management
- **No Dependencies**: Pure HTML/CSS/JavaScript - no frameworks or build tools required
- **Real-time Updates**: Changes in admin panel instantly reflect on main website

## 🌐 GitHub Pages Hosting Guide

### Step-by-Step Instructions

1. **Create GitHub Repository**
   ```bash
   # Initialize git in your project folder
   git init
   
   # Add all files
   git add .
   
   # Commit changes
   git commit -m "Initial commit"
   
   # Create new repository on GitHub (follow GitHub's instructions)
   
   # Add remote origin
   git remote add origin https://github.com/yourusername/your-repo-name.git
   
   # Push to GitHub
   git branch -M main
   git push -u origin main
   ```

2. **Enable GitHub Pages**
   - Go to your repository on GitHub
   - Click "Settings" tab
   - Scroll down to "Pages" section in left sidebar
   - Under "Source", select "Deploy from a branch"
   - Choose "main" branch and "/ (root)" folder
   - Click "Save"

3. **Wait for Deployment**
   - GitHub will process your site (1-5 minutes)
   - You'll see a success message with your site URL
   - URL format: `https://yourusername.github.io/your-repo-name`

4. **Verify Deployment**
   - Visit your site URL
   - Test both `index.html` and `admin.html`
   - Verify admin panel functionality works with LocalStorage

### Custom Domain (Optional)
1. Create `CNAME` file in root directory:
   ```
   yourdomain.com
   ```
2. Push to GitHub
3. Configure DNS settings with your domain provider
4. Enable HTTPS in GitHub Pages settings

### Troubleshooting
- **404 Error**: Ensure `index.html` is in root directory
- **Admin Panel Not Working**: Check browser console for errors
- **Images Not Loading**: Verify image URLs are correct
- **Slow Loading**: Optimize images and check network connection

## 🎨 Customization

### Colors
Edit CSS variables in `index.html`:
```css
:root {
  --primary-color: #1e40af;
  --primary-hover: #1e3a8a;
  --secondary-color: #0ea5e9;
  --text-color: #0f172a;
  --bg-color: #f8fafc;
}
```

### Fonts
Update Google Fonts link in `<head>`:
```html
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&family=Playfair+Display:wght@700&display=swap" rel="stylesheet">
```

### Content
- Edit JSON files in `src/data/` for content updates
- Use `admin.html` for easy content management
- Export/import data for backup and migration

## 📞 Support

For technical support or questions:
- Email: sales@alliedcochin.com
- Phone: +91 98460 12345
- Address: Mukkadackal Buildings, Hill Palace Rd, Thrippunithura, Kochi, Kerala 682301

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Allied Agencies Cochin** - Trusted Water Pump Solutions Since 1973