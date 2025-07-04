# The Fives Diet Website

A modern, responsive website for The Fives Diet - a simple approach to sustainable eating based on the power of five.

## The Diet Concept

**Five days a week, eat fifty calories at a time, up to five hundred calories, consuming under five thousand calories per week.**

## Technology Stack

- **Astro** - Static site generator for fast, modern web development
- **Tailwind CSS** - Utility-first CSS framework for responsive design
- **TypeScript** - Type-safe JavaScript development

## Development

### Prerequisites

- Node.js 18+ 
- npm or yarn

### Getting Started

1. Install dependencies:
```bash
npm install
```

2. Start the development server:
```bash
npm run dev
```

3. Open [http://localhost:4321](http://localhost:4321) in your browser

### Available Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run preview` - Preview production build locally
- `npm run deploy` - Build and deploy to GitHub Pages

## Deployment to GitHub Pages

This site is configured to deploy to the custom domain `dreadpiraterobertson.com` via GitHub Pages.

### Setup Instructions

1. **Create GitHub Repository**
   - Create a new repository on GitHub
   - Push this code to the repository

2. **Configure GitHub Pages**
   - Go to repository Settings → Pages
   - Set Source to "Deploy from a branch"
   - Select the `gh-pages` branch
   - The CNAME file will automatically configure the custom domain

3. **DNS Configuration**
   - Configure your DNS provider to point `dreadpiraterobertson.com` to GitHub Pages
   - Add CNAME record: `dreadpiraterobertson.com` → `yourusername.github.io`
   - Add A records for apex domain:
     - `185.199.108.153`
     - `185.199.109.153` 
     - `185.199.110.153`
     - `185.199.111.153`

4. **Deploy**
   ```bash
   npm run deploy
   ```

### Manual Deployment

If you prefer to deploy manually:

1. Build the site:
   ```bash
   npm run build
   ```

2. Deploy the `dist` folder to GitHub Pages:
   ```bash
   npx gh-pages -d dist
   ```

## Site Structure

```
src/
├── layouts/
│   └── BaseLayout.astro    # Base HTML layout with SEO
├── pages/
│   └── index.astro         # Homepage
└── styles/
    └── global.css          # Global Tailwind CSS
public/
├── CNAME                   # Custom domain configuration
└── fives-diet-logo.svg     # Site logo
```

## Features

- 📱 **Responsive Design** - Optimized for all devices
- 🌙 **Dark Mode Support** - Automatic dark/light theme switching
- ⚡ **Fast Loading** - Static site generation with Astro
- 🔍 **SEO Optimized** - Meta tags, Open Graph, and sitemap
- ♿ **Accessible** - WCAG compliant design patterns

## Customization

The site uses Tailwind CSS for styling. You can customize:

- **Colors**: Edit the gradient and color scheme in `index.astro`
- **Typography**: Modify font sizes and weights throughout
- **Layout**: Adjust spacing and grid layouts
- **Content**: Update the diet information and benefits

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test locally with `npm run dev`
5. Submit a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

---

**Disclaimer**: This diet plan is for informational purposes only. Please consult with a healthcare professional before starting any new diet regimen.