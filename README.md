# MarkSite 📄✨

A beautiful, modern markdown-to-HTML renderer with advanced features including dark/light themes, responsive design, and table of contents navigation.

![License](https://img.shields.io/badge/license-GPL%20v3-blue.svg)
![Version](https://img.shields.io/badge/version-1.2-green.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)

## 🌟 Features

- **📱 Responsive Design**: Works perfectly on desktop, tablet, and mobile devices
- **🌙 Dark/Light Theme**: Automatic theme detection with manual toggle support
- **📋 Table of Contents**: Auto-generated navigation sidebar with smooth scrolling
- **🎨 Modern UI**: Clean, professional design with smooth animations
- **⚡ Fast Loading**: Optimized for performance with minimal dependencies
- **🔗 URL Support**: Load any markdown file via URL parameter
- **♿ Accessible**: Built with accessibility in mind
- **📚 GitHub Flavored Markdown**: Full GFM support including tables, code blocks, and more

## 🚀 Live Demo

Visit the live demo at: **https://marksite.free.nf/**

## 📖 Usage

### Basic Usage

Simply visit the website to view the default markdown document.

### Load Custom Markdown

Add a `url` parameter to load your own markdown file:

```
https://marksite.free.nf/?url=https://raw.githubusercontent.com/yourusername/yourrepo/main/README.md
```

### Examples

```bash
# Load a GitHub README
https://marksite.free.nf/?url=https://raw.githubusercontent.com/microsoft/vscode/main/README.md

# Load any public markdown file
https://marksite.free.nf/?url=https://example.com/documentation.md
```

## 🛠️ Installation

### Option 1: Direct Download

1. Download the `index.html` file
2. Upload to your web hosting service
3. Access via your domain

### Option 2: Clone Repository

```bash
git clone https://github.com/yourusername/marksite.git
cd marksite
# Upload index.html to your hosting service
```

### Option 3: Local Development

```bash
# Serve locally with Python
python -m http.server 8000

# Or with Node.js
npx http-server

# Then visit http://localhost:8000
```

## ⚙️ Configuration

The application automatically detects the best configuration, but you can customize:

### Default Markdown URL

Edit line 674 in `index.html`:

```javascript
return urlFromParam || 'https://raw.githubusercontent.com/your-repo/main/your-file.md';
```

### Theme Settings

The app automatically detects system theme preference. Users can toggle manually using:
- Click the theme button (🌙/☀️)
- Keyboard shortcut: `Ctrl/Cmd + Shift + D`

### Table of Contents

The TOC is automatically generated based on heading structure:
- Multiple H1 tags → Uses H1 for navigation
- Single H1 + H2 tags → Uses H2 for navigation  
- No H2 tags → Falls back to H3 or H4

## 🎨 Customization

### CSS Variables

Modify the CSS variables in the `:root` selector to customize colors:

```css
:root {
    --bg-primary: #ffffff;
    --text-primary: #24292f;
    --text-accent: #0969da;
    /* ... more variables */
}
```

### Adding Custom Styles

Add your custom CSS after the existing styles in the `<style>` section.

## 🔧 Technical Details

### Dependencies

- **Marked.js**: Markdown parsing (loaded from CDN)
- **No other external dependencies**

### Browser Support

- ✅ Chrome 60+
- ✅ Firefox 60+
- ✅ Safari 12+
- ✅ Edge 79+
- ✅ Mobile browsers

### Performance Features

- Lazy loading for large documents
- Smooth scrolling with intersection observer
- Optimized CSS animations
- Minimal JavaScript footprint

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

### Development Setup

1. Fork the repository
2. Make your changes to `index.html`
3. Test locally
4. Submit a pull request

### Contribution Guidelines

- Follow existing code style
- Test on multiple browsers
- Ensure responsive design works
- Update documentation if needed

## 📄 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](https://github.com/nguyenhhoa03/md2web/blob/main/LICENSE) section below for details.

## 🛡️ Security

- No user data is stored
- All markdown processing happens client-side
- CORS-enabled for loading external markdown files
- No server-side processing required

## 📈 Version History

| Version | Release Date | Key Features |
|---------|-------------|--------------|
| **v1.2** | Current | 🔗 URL parameter support, Mobile improvements |
| **v1.1** | Previous | 📋 Auto table of contents |
| **v1.0** | Initial | 📄 Basic markdown viewing, 🌙 Theme support |

## 🆘 Support

If you encounter any issues or have questions:

1. Check the browser console for errors
2. Ensure the markdown URL is publicly accessible
3. Verify CORS headers are set correctly on the markdown source
4. Try with different markdown files to isolate the issue

## 🌍 Hosting Recommendations

MarkSite works with any static hosting service:

- **GitHub Pages**: Free hosting for GitHub repositories
- **Netlify**: Easy deployment with continuous integration
- **Vercel**: Fast global CDN
- **Firebase Hosting**: Google's hosting platform
- **Any static hosting**: Upload `index.html` and go!

## 📚 Markdown Support

MarkSite supports all GitHub Flavored Markdown features:

- ✅ Headers (H1-H6)
- ✅ **Bold** and *italic* text
- ✅ Links and images
- ✅ Code blocks with syntax highlighting
- ✅ Tables
- ✅ Blockquotes
- ✅ Lists (ordered and unordered)
- ✅ Horizontal rules
- ✅ Strikethrough text
- ✅ Task lists
- ✅ Emoji support

## 🔮 Future Enhancements

- [ ] PDF export functionality
- [ ] Print-optimized styles
- [ ] Search functionality
- [ ] Multiple theme options
- [ ] Offline support with service worker
- [ ] Custom CSS injection via URL parameters

---

**Made with ❤️ for the markdown community**

*Host your markdown files beautifully with MarkSite!*
