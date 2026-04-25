# Hikari - Quote Generator 💎

A modern, aesthetically beautiful quote generator with a focus on money mindset, business, and luxury lifestyle quotes.

## ✨ Features

- 🎯 **16 Powerful Quotes** - Money mindset, business, and peak performance quotes
- 🖼️ **13 Beautiful Backgrounds** - High-quality images that rotate with each quote
- 📤 **Upload Custom Background** - Users can upload their own images (session-based, not saved)
- 📥 **Download as Image** - Save quotes as PNG images
- 🎨 **Modern UI** - Glassmorphism design with smooth animations
- 📱 **Fully Responsive** - Works on all devices
- ⚡ **Zero Dependencies** - Pure HTML, CSS, and JavaScript (only html2canvas for download)

## 🚀 Live Demo

Visit: **https://ayushauralabs.github.io/Hikari/**

## 📁 Project Structure

```
Hikari/
├── index.html          # Main application file
├── images/             # Background images (13 files)
│   ├── pexels-alex-ning-523843601-37069218.jpg
│   ├── pexels-alexfu-945966.jpg
│   └── ... (11 more images)
└── README.md           # This file
```

## 🛠️ How to Use Locally

1. Clone or download the repository
2. Make sure the `images` folder contains all 13 image files
3. Open `index.html` in your web browser
4. Click "Generate Quote" to cycle through quotes and backgrounds

## 💻 Features Breakdown

### Generate Quote Button
- Shows a new random quote from the collection
- Randomly selects a background image from the images folder
- Smooth fade transitions

### Upload Background Button (📁)
- Located at bottom right
- Allows users to upload any image temporarily
- Image is stored only in browser memory (not saved)
- Next "Generate Quote" will use the uploaded image

### Reset Button (✕)
- Located at top right (red circle)
- Clears uploaded images and returns to random image cycling
- Useful for switching back to the curated background images

### Download Image Button
- Saves the current quote and background as a PNG image
- Works with both pre-loaded and user-uploaded images
- Uses html2canvas library for image capture

## 🔧 Customization

### Add More Quotes
Edit the `quotes` array in the JavaScript section:
```javascript
const quotes = [
    {
        text: "Your quote here",
        author: "Author Name"
    },
    // Add more quotes...
];
```

### Add More Background Images
1. Place images in the `images/` folder
2. Add the filename to the `backgrounds` array:
```javascript
const backgrounds = [
    "url('images/your-image-name.jpg')",
    // Add more images...
];
```

## 📋 Quote Categories

The current quotes focus on:
- **Money Mindset** - Financial wisdom and wealth building
- **Business & Leadership** - Entrepreneurship and success strategies
- **Peak Performance** - Discipline and excellence
- **Luxury & Lifestyle** - Aspirational quotes
- **Personal Growth** - Self-improvement and motivation

## 🌐 Deployment to GitHub Pages

### Prerequisites
- A GitHub repository named `Hikari` (or your preferred name)
- The repository should be public

### Steps
1. **Upload Files to GitHub**
   - Push `index.html` to your repository
   - **IMPORTANT:** Push the entire `images/` folder with all image files

2. **Enable GitHub Pages**
   - Go to Repository Settings → Pages
   - Set Source to `main` branch
   - Your site will be available at: `https://yourusername.github.io/Hikari/`

3. **Verify Images are Loading**
   - Check the `images/` folder exists in your repository
   - All 13 image files should be present
   - If images aren't loading, ensure the folder structure matches the code references

### Troubleshooting GitHub Pages

**Images Not Loading?**
- ✅ Verify `images/` folder exists in your GitHub repository
- ✅ Check that all image files are actually pushed (not just the folder)
- ✅ Use `git add images/` and `git commit -m "Add images"`
- ✅ Wait 1-2 minutes for GitHub Pages to rebuild

**Quick Fix Commands:**
```bash
# Make sure images are tracked
git add images/
git add *.html
git commit -m "Update project with images"
git push origin main
```

## 📱 Browser Compatibility

- Chrome/Edge: ✅ Full support
- Firefox: ✅ Full support
- Safari: ✅ Full support
- Mobile Browsers: ✅ Fully responsive

## 📝 License

Free to use and modify for personal or commercial projects.

## 🎨 Design Credits

- **Fonts:** Playfair Display (quotes), Poppins (UI)
- **Icons:** Unicode symbols
- **Background Images:** Pexels (free stock photos)
- **Design Pattern:** Glassmorphism

## 💡 Tips for Best Experience

1. **Mobile:** The design is fully responsive - looks great on phones and tablets
2. **Sharing:** Download quotes as images and share on social media
3. **Custom Branding:** Upload your own logo/branding images
4. **Printing:** Downloaded images can be printed in high quality

---

**Made with ❤️ by AyushAuraLabs**
