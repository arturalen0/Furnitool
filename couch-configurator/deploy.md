# Deployment Guide

## Quick Deploy to Vercel

### Option 1: GitHub Integration (Recommended)

1. Push your code to GitHub
2. Go to [vercel.com](https://vercel.com)
3. Click "New Project"
4. Import your GitHub repository
5. Deploy automatically - no configuration needed!

### Option 2: Vercel CLI

```bash
# Install Vercel CLI
npm i -g vercel

# Deploy from project directory
cd couch-configurator
vercel

# Follow the prompts
```

### Option 3: Drag & Drop

1. Go to [vercel.com](https://vercel.com)
2. Drag the `couch-configurator` folder to the deployment area
3. Deploy instantly

## Other Hosting Options

### Netlify

1. Drag folder to [netlify.com/drop](https://netlify.com/drop)
2. Or connect GitHub repository
3. Deploy automatically

### GitHub Pages

1. Push to GitHub repository
2. Go to Settings > Pages
3. Select source branch
4. Enable HTTPS (required for AR)

### Traditional Web Hosting

1. Upload all files via FTP/SFTP
2. Ensure HTTPS is enabled
3. Configure MIME types:
   - `.glb` → `model/gltf-binary`
   - `.gltf` → `model/gltf+json`

## Post-Deployment Checklist

✅ **HTTPS Enabled** - Required for AR functionality
✅ **Mobile Testing** - Test AR on actual mobile devices
✅ **QR Code Working** - Verify QR codes generate and scan properly
✅ **3D Model Loading** - Check all textures load correctly
✅ **Cross-browser Testing** - Test on different browsers
✅ **Performance** - Check loading times and responsiveness

## Custom Domain Setup

### Vercel

1. Go to Project Settings > Domains
2. Add your custom domain
3. Configure DNS records as shown

### Cloudflare (Optional)

- Add CDN and additional performance optimizations
- Enable additional security features
- Optimize image delivery

## Environment Variables

No environment variables needed - this is a static site!

## Monitoring

Consider adding:

- Google Analytics for usage tracking
- Error monitoring (Sentry)
- Performance monitoring (Web Vitals)

## Troubleshooting

### AR Not Working

- Ensure HTTPS is enabled
- Check mobile browser compatibility
- Verify model-viewer scripts load correctly

### 3D Model Not Loading

- Check file paths are correct
- Verify GLB file is not corrupted
- Check browser console for errors

### QR Code Issues

- Verify QR API is accessible
- Check network connectivity
- Test fallback AR links manually
