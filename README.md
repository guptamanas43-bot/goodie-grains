# Food Brand Static Website

A professional static website for a food brand with product showcase and Amazon integration.

## Features

- **Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **Navigation Tabs**: Home, About Us, Products, and Bulk Orders
- **Amazon Integration**: Direct links to purchase products on Amazon
- **Modern UI**: Clean, professional design with smooth animations
- **Static HTML/CSS/JS**: No backend required, perfect for GitHub Pages

## File Structure

```
.
├── index.html          # Home page
├── about.html          # About Us page
├── products.html       # Products page
├── bulk-orders.html    # Bulk Orders page
├── styles.css          # Main stylesheet
├── script.js           # JavaScript for interactivity
├── images/             # Directory for product images
└── README.md           # This file
```

## Setup Instructions

### 1. Add Your Product Images

Place your product images in the `images/` folder with the following names:
- `product1.jpg`
- `product2.jpg`
- `product3.jpg`
- `product4.jpg`
- `product5.jpg`
- `product6.jpg`

Or update the image paths in the HTML files to match your image names.

### 2. Customize Content

Edit the following in the HTML files:

**Brand Name**: Replace "Your Food Brand" with your actual brand name in all HTML files

**Product Information**: Update product names, descriptions, and Amazon links in:
- `index.html` (Featured Products section)
- `products.html` (All product cards)

**Amazon Links**: Replace `https://www.amazon.com/your-product-link` with your actual Amazon product URLs

**Contact Information**: Update email and phone in the footer of all pages

**About Us Content**: Customize the story, values, and information in `about.html`

### 3. Deploy to GitHub Pages

#### Step 1: Create a GitHub Repository

```bash
# Initialize git repository (if not already done)
git init

# Add all files
git add .

# Commit files
git commit -m "Initial commit: Food brand website"

# Create a new repository on GitHub (via web interface)
# Then connect your local repo to GitHub:
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

#### Step 2: Enable GitHub Pages

1. Go to your repository on GitHub
2. Click on **Settings**
3. Scroll down to **Pages** section (in the left sidebar)
4. Under **Source**, select **main** branch
5. Select **/ (root)** folder
6. Click **Save**

#### Step 3: Access Your Website

Your website will be available at:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

It may take a few minutes for the site to be published.

## Customization Tips

### Change Colors

Edit `styles.css` to change the color scheme:
- Primary color: `#667eea` (purple gradient)
- Secondary color: `#f39c12` (orange/gold)
- Dark background: `#2c3e50`
- Amazon button: `#FF9900`

### Add More Products

1. Copy a product card div in `products.html`
2. Update the image source, product name, description, and Amazon link
3. Add corresponding image to the `images/` folder

### Modify Layout

The website uses CSS Grid for responsive layouts. Adjust grid settings in `styles.css`:
```css
.product-grid {
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
}
```

## Form Integration (Bulk Orders)

The contact form currently shows an alert. To make it functional:

### Option 1: Formspree (Recommended for static sites)
1. Sign up at [Formspree.io](https://formspree.io)
2. Create a new form
3. Update the form tag in `bulk-orders.html`:
```html
<form action="https://formspree.io/f/YOUR-FORM-ID" method="POST" class="contact-form">
```

### Option 2: Google Forms
1. Create a Google Form
2. Embed it in `bulk-orders.html`

### Option 3: Netlify Forms
If you deploy to Netlify instead of GitHub Pages, add `netlify` attribute to the form.

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile browsers

## License

This template is free to use for your food brand website.

## Support

For issues or questions about deployment, refer to:
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Git Basics](https://git-scm.com/book/en/v2/Getting-Started-Git-Basics)

---

**Note**: Remember to replace all placeholder content with your actual brand information before deploying!

