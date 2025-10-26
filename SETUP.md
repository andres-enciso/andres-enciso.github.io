# GitHub Pages Setup Guide

This guide will help you configure and deploy your portfolio site on GitHub Pages.

## 📋 Prerequisites

1. A GitHub account
2. Git installed on your computer
3. (Optional) Ruby and Jekyll for local testing

## 🚀 Quick Start

### Step 1: Configure GitHub Pages

1. Go to your repository on GitHub: `https://github.com/andres-enciso/andres-enciso.github.io`
2. Click on **Settings** (top right)
3. Scroll down to **Pages** section (left sidebar)
4. Under **Source**, select:
   - Branch: `main`
   - Folder: `/ (root)`
5. Click **Save**

### Step 2: Update Your Information

Edit the following files with your personal information:

#### `_config.yml`
```yaml
email: your.email@example.com        # Your email
linkedin_username: your-linkedin-username  # Your LinkedIn username
```

#### `index.md`
Update the following sections:
- LinkedIn URL (bottom of the file)
- Email address (bottom of the file)
- Add your actual projects and experience

### Step 3: Push Your Changes

```bash
# Add all files
git add .

# Commit your changes
git commit -m "Configure GitHub Pages with Jekyll"

# Push to GitHub
git push origin main
```

### Step 4: Access Your Site

Your site will be available at: `https://andres-enciso.github.io`

Note: It may take 1-2 minutes for GitHub Pages to build and deploy your site.

## 🛠️ Local Development (Optional)

To test your site locally before pushing:

### Install Dependencies

```bash
# Install Ruby (if not already installed)
# Windows: Download from https://rubyinstaller.org/
# Mac: brew install ruby
# Linux: sudo apt-get install ruby-full

# Install Bundler
gem install bundler

# Install project dependencies
bundle install
```

### Run Local Server

```bash
# Start Jekyll server
bundle exec jekyll serve

# Your site will be available at http://localhost:4000
```

## 📁 Project Structure

```
andres-enciso.github.io/
├── _layouts/           # HTML templates
│   └── default.html    # Main layout template
├── assets/
│   ├── css/
│   │   └── style.css   # Custom styles
│   └── js/
│       └── main.js     # Custom JavaScript
├── _config.yml         # Jekyll configuration
├── index.md            # Homepage content
├── README.md           # Repository description
├── Gemfile             # Ruby dependencies
└── .gitignore          # Git ignore rules
```

## 🎨 Customization

### Colors and Styling

Edit `assets/css/style.css` to change:
- Color scheme (`:root` variables)
- Typography
- Layouts and spacing

### Layout

Edit `_layouts/default.html` to modify:
- Header and navigation
- Footer
- Meta tags

### Content

Edit `index.md` to update:
- About section
- Tech stack
- Projects
- Contact information

## 🔍 Troubleshooting

### Site not showing up?
- Wait 1-2 minutes for GitHub to build
- Check Settings > Pages to ensure it's enabled
- Verify your repository name is `andres-enciso.github.io`

### Styling not working?
- Clear your browser cache
- Check that CSS file paths are correct in `_layouts/default.html`

### Local build errors?
- Make sure you have Ruby 2.7 or higher: `ruby -v`
- Reinstall dependencies: `bundle install`

## 📚 Additional Resources

- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Jekyll Documentation](https://jekyllrb.com/docs/)
- [Markdown Guide](https://www.markdownguide.org/)

## 📝 Next Steps

1. ✅ Configure GitHub Pages
2. ✅ Update personal information
3. ✅ Push changes to GitHub
4. 📝 Add your actual projects
5. 📝 Write blog posts (create `_posts/` directory)
6. 📝 Add a custom domain (optional)

---

Good luck with your portfolio site! 🚀
