---
title: Getting Started with Jekyll & Chirpy Theme
date: 2026-05-12 10:00:00 +0000
categories: [Tutorial, Jekyll]
tags: [jekyll, github-pages, blogging, tutorial, setup]
excerpt: "A complete guide to setting up your Jekyll blog with the Chirpy theme on GitHub Pages. Learn how to create posts, customize your site, and go live."
---

# Getting Started with Jekyll & Chirpy Theme

Setting up a blog doesn't have to be complicated. In this guide, we'll walk through setting up a beautiful, fully-featured blog using **Jekyll** and the **Chirpy theme** on GitHub Pages—all for free! ✨

## 🎯 What We'll Cover

- ✅ Jekyll basics and structure
- ✅ Chirpy theme features
- ✅ Creating and publishing blog posts
- ✅ Customizing your site
- ✅ Deploying to GitHub Pages

## 📋 Prerequisites

- GitHub account
- Git installed locally
- Basic command line knowledge
- Ruby and Bundler (for local development)

## 🚀 Step 1: Create Your Repository

1. Create a new repository named: `yourusername.github.io`
2. Clone it locally:

```bash
git clone https://github.com/yourusername/yourusername.github.io
cd yourusername.github.io
```

## 📦 Step 2: Set Up Jekyll

Initialize Jekyll in your repository:

```bash
# Create a new Jekyll site (or use existing files)
jekyll new . --force

# Or manually create the structure
mkdir _posts _layouts _includes _sass assets
```

## 🎨 Step 3: Add Chirpy Theme

Update your `Gemfile`:

```ruby
gem "jekyll-theme-chirpy", "~> 6.0"

group :jekyll_plugins
  gem "jekyll-paginate", "~> 1.1"
  gem "jekyll-redirect-from", "~> 0.16"
  gem "jekyll-seo-tag", "~> 2.8"
  gem "jekyll-archives", "~> 2.2"
  gem "jekyll-sitemap", "~> 1.4"
end
```

Install dependencies:

```bash
bundle install
```

## ⚙️ Step 4: Configure Your Site

Create `_config.yml`:

```yaml
# Basic Settings
title: Your Blog Title
tagline: Your tagline here
description: Your description
url: https://yourusername.github.io

# Author
author:
  name: Your Name
  email: your@email.com

# Theme
theme: jekyll-theme-chirpy

# Plugins
plugins:
  - jekyll-paginate
  - jekyll-seo-tag
  - jekyll-archives

# Pagination
paginate: 10
paginate_path: /blog/page:num/

# Markdown
markdown: kramdown
```

## 📝 Step 5: Create Your First Post

Create a new file in `_posts/`:

**Filename Format:** `YYYY-MM-DD-title.md`

Example: `_posts/2026-05-12-my-first-post.md`

```markdown
---
title: My First Post
date: 2026-05-12 10:00:00 +0000
categories: [Getting Started]
tags: [jekyll, blogging]
---

# My First Blog Post

Write your content here using Markdown!

## Section Heading

Some paragraph text with **bold** and *italic* formatting.

### Code Example

```python
def hello_world():
    print("Hello, World!")
```
```

## 🏃 Step 6: Test Locally

Run the Jekyll development server:

```bash
bundle exec jekyll serve
```

Visit `http://localhost:4000` in your browser!

## 📤 Step 7: Deploy to GitHub Pages

1. Push your changes:

```bash
git add .
git commit -m "Initial Jekyll setup with Chirpy theme"
git push origin main
```

2. Go to your repo **Settings → Pages**
3. Set **Source** to "Deploy from a branch"
4. Select **main** branch
5. Click **Save**

Your site will be live at `https://yourusername.github.io` in about 5 minutes! 🎉

## ✨ Chirpy Theme Features

The Chirpy theme provides amazing features out of the box:

### 🎨 Beautiful Design
- Responsive layout
- Light/Dark mode
- Smooth animations
- Professional aesthetics

### 🔍 Built-in Search
- Full-text search
- Tag & category filtering
- Smart suggestions

### 📱 Mobile Optimized
- Touch-friendly navigation
- Responsive images
- Fast loading

### ⚡ Performance
- Optimized CSS/JS
- Image lazy loading
- Fast builds

### 🔐 SEO
- Automatic sitemaps
- Meta tags
- Schema markup

## 📚 Creating Different Post Types

### Tutorial Post

```markdown
---
title: Tutorial: How to Build X
date: 2026-05-13 10:00:00 +0000
categories: [Tutorial]
tags: [tutorial, step-by-step]
---

## Prerequisites
- Item 1
- Item 2

## Step 1: Setup

## Step 2: Implementation

## Step 3: Testing
```

### Quick Tip

```markdown
---
title: "Quick Tip: Useful Command"
date: 2026-05-13 10:00:00 +0000
categories: [Tips]
tags: [tip, productivity]
---

```

### Deep Dive Article

```markdown
---
title: "Deep Dive: Understanding XYZ"
date: 2026-05-13 10:00:00 +0000
categories: [Technical]
tags: [advanced, architecture]
---
```

## 🎯 Best Practices

### File Naming
✅ `2026-05-12-how-to-build-android-app.md`  
❌ `my-post.md`

### Front Matter
Always include:
- `title` – Post title
- `date` – Publication date
- `categories` – 1-2 categories
- `tags` – 3-5 relevant tags

### Content Structure
1. **Title** (H1)
2. **Introduction** (brief overview)
3. **Main Content** (H2 sections)
4. **Conclusion** (summary or next steps)

## 🚀 Next Steps

1. **Customize Colors** – Edit `_sass/colors/` files
2. **Add Navigation** – Update `_config.yml`
3. **Write More Posts** – Build your content library
4. **Enable Comments** – Configure Disqus or Utterances
5. **Set Up Analytics** – Track your audience

## 🔗 Useful Resources

- [Jekyll Documentation](https://jekyllrb.com/)
- [Chirpy Theme GitHub](https://github.com/cotes2020/jekyll-theme-chirpy)
- [Markdown Guide](https://www.markdownguide.org/)
- [GitHub Pages Help](https://docs.github.com/en/pages)

## 💡 Tips for Success

✅ Write consistently – Post on a regular schedule  
✅ Use categories & tags – Help readers find content  
✅ Include code examples – Show, don't just tell  
✅ Add images – Break up text visually  
✅ Optimize for SEO – Use good titles and descriptions  
✅ Engage with readers – Respond to comments  

---

**You're all set! Start writing and let your blog shine!** ✨

Happy blogging! 🚀

---

*Posted on May 12, 2026 | [Back to Blog](/blog/)*
