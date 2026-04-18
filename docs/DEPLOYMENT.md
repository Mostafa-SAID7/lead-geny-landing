# Deployment Guide

## Netlify Deployment

This Angular application is configured for seamless deployment on Netlify.

### Configuration

The `netlify.toml` file contains the build configuration:

```toml
[build]
  command = "npm run build"
  publish = "dist/lead-gen-landing/browser"

[build.environment]
  NODE_VERSION = "22.14.0"

[[redirects]]
  from = "/*"
  to = "/index.html"
  status = 200
```

> **Note:** The `NODE_VERSION` environment variable ensures Netlify uses the correct Node.js version (v22.14.0) required by Angular 21.

### Deployment Steps

1. **Connect Repository**: Link your GitHub repository to Netlify
2. **Build Settings**: The settings are automatically configured via `netlify.toml`
3. **Deploy**: Push to your main branch to trigger automatic deployment

### Manual Deployment

```bash
# Install Netlify CLI
npm install -g netlify-cli

# Build the project
npm run build

# Deploy
netlify deploy --prod --dir=dist/lead-gen-landing/browser
```

### Environment Variables

If your application requires environment variables, add them in:
- Netlify Dashboard → Site Settings → Environment Variables

### Troubleshooting

**Issue**: Build fails with publish directory error
**Solution**: Ensure `netlify.toml` is present with correct publish path

**Issue**: 404 on page refresh
**Solution**: The redirect rule in `netlify.toml` handles SPA routing
