# Indabo - AI-Powered Career Development Platform

Indabo is a modern career development platform that leverages artificial intelligence to help users build their careers, create professional resumes, and receive personalized career guidance.

## 🌟 Features

### Core Functionalities

- **AI-Driven Career Blueprint**: Personalized career path planning and step-by-step guidance
- **CV/Resume Builder**: Create professional resumes that stand out to employers
- **Career Coach**: 24/7 AI-powered career guidance and job advice
- **Learning Platform**: Access to top courses for skill development and career advancement

### Key Benefits

- Personalized career planning
- 24/7 AI coaching support
- Professional resume building
- Interview preparation guidance
- Skill development resources
- Career advancement tools

## 🏗️ Project Structure

```
indabo/
├── hugo.yaml           # Main configuration file
├── static/            # Static assets
│   ├── images/        # Image assets
│   │   ├── logos/     # Logo files
│   │   └── illustrations/  # Illustration assets
├── content/           # Content files
│   ├── features/      # Features pages
│   ├── pricing/       # Pricing pages
│   └── blog/          # Blog posts
└── layouts/           # Hugo layout templates
```

## 📚 Important Files and Hugo Concepts

### Configuration Files

- `hugo.yaml`: The main configuration file that defines:
  - Site metadata (title, baseURL, language)
  - Module settings
  - Google Analytics configuration
  - Content parameters (navigation, hero section, features)
  - Theme settings and customizations

### Content Organization

- `content/`: Contains all the content of your site
  - `_index.md`: The homepage content
  - `features/`: Feature pages and their content
  - `pricing/`: Pricing information and plans
  - `blog/`: Blog posts organized by date or category

### Layout Templates

- `layouts/`: Contains the HTML templates that define how content is rendered
  - `_default/`: Default templates for different content types
  - `partials/`: Reusable template components
  - `shortcodes/`: Custom shortcodes for content formatting

### Static Assets

- `static/`: Contains all static files that are served directly
  - `images/`: All image assets
  - `css/`: Custom stylesheets
  - `js/`: JavaScript files
  - `fonts/`: Custom fonts

### Key Hugo Concepts

#### Content Types

- **Pages**: Regular content pages
- **Posts**: Blog posts with dates and categories
- **Sections**: Groups of content (e.g., features, pricing)
- **Taxonomies**: Content organization (categories, tags)

#### Front Matter

Each content file starts with front matter (YAML, TOML, or JSON) that defines:

```yaml
---
title: 'Page Title'
date: 2024-03-20
draft: false
---
```

#### Template Hierarchy

Hugo follows a specific template lookup order:

1. Layout specific to the content type
2. Section template
3. Default template
4. Base template

#### Shortcodes

Custom shortcodes for dynamic content:

```markdown
{{< feature title="AI Career Coach" icon="laptop-cloud" >}}
```

#### Content Organization

- Use `_index.md` files to define section pages
- Organize content in subdirectories for better structure
- Use front matter to control page behavior and metadata

### Development Workflow

1. **Content Creation**

   ```bash
   hugo new content features/ai-coach.md
   hugo new content blog/my-first-post.md
   ```

2. **Content Preview**

   ```bash
   hugo server -D --navigateToChanged
   ```

3. **Building for Production**

   ```bash
   hugo --minify
   ```

4. **Content Management**
   - Use `draft: true` in front matter for unpublished content
   - Set `publishDate` for future publishing
   - Use `weight` to control menu order

### Best Practices

- Keep content and presentation separate
- Use partial templates for reusable components
- Implement responsive images with Hugo's image processing
- Use data files for structured content
- Leverage Hugo's built-in caching for performance

## 🚀 Getting Started

### Prerequisites

- Hugo (latest version)
- Git

### Local Development

1. Clone the repository:

   ```bash
   git clone [repository-url]
   cd indabo
   ```

2. Install dependencies:

   ```bash
   hugo mod get -u
   ```

3. Run the development server:

   ```bash
   hugo server -D
   ```

4. Visit `http://localhost:1313` to view the site

## 🌐 Deployment

The site is deployed at:

- Landing Page: www.indabo.com
- Application: app.indabo.com

## 🛠️ Technology Stack

- **Framework**: Hugo (Static Site Generator)
- **Frontend**: Custom CSS with Bulma framework
- **Analytics**: Google Analytics integration
- **Content Management**: Markdown-based content system

## 📝 Content Management

The site uses Hugo's content management system with the following structure:

- Features and pricing pages are managed through the `content/` directory
- Blog posts are stored in `content/blog/`
- Static assets are managed in the `static/` directory

## 🔒 Security

- All sensitive data is handled through secure connections
- API keys and credentials are managed through environment variables
- HTTPS is enforced across all domains

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is proprietary software. All rights reserved.

## 📞 Contact

For any inquiries, please reach out through the contact form on the website or email [contact@indabo.com](mailto:contact@indabo.com).

---

Built with ❤️ by the Indabo Team
