# 3D Couch Configurator with AR Support

A professional 3D furniture configurator that allows users to customize couch materials on desktop and view them in AR on mobile devices.

## Features

### Desktop Experience

- **Real-time 3D Configurator** - Interactive Three.js-powered 3D model
- **Material Customization** - Choose from multiple fabric, stitch, and leg options
- **Professional Lighting** - Cinema-quality lighting with shadows and effects
- **Smooth Controls** - Professional camera controls with constraints
- **QR Code Generation** - Real-time QR codes for mobile AR viewing

### Mobile AR Experience

- **AR Viewer** - View configured couch in your actual space
- **Cross-platform** - Works on iOS (ARKit) and Android (ARCore)
- **Configuration Sync** - Maintains exact material selections from desktop
- **Share Functionality** - Share configurations with others

## Technology Stack

- **Three.js** - 3D rendering and controls
- **Model-viewer** - AR functionality
- **WebXR** - AR standards compliance
- **Vanilla JavaScript** - No framework dependencies
- **GLB/GLTF** - 3D model format

## Deployment

### Vercel (Recommended)

1. Connect your repository to Vercel
2. Deploy automatically with zero configuration
3. Vercel handles static file serving and CDN

### Manual Deployment

1. Upload all files to your web server
2. Ensure HTTPS is enabled (required for AR)
3. Configure proper MIME types for .glb files

## File Structure

```
couch-configurator/
├── index.html              # Main 3D configurator
├── ar-viewer.html          # Mobile AR viewer
├── model-viewer-version.html # Alternative model-viewer version
├── couch.glb              # 3D couch model
├── textures/              # PBR texture maps
│   ├── fabrics/           # Fabric texture sets
│   └── legs/              # Leg material textures
├── vercel.json            # Vercel configuration
├── package.json           # Project metadata
└── README.md              # This file
```

## Usage

1. **Configure on Desktop** - Select materials using the control panel
2. **Generate QR Code** - QR code updates automatically with selections
3. **Scan with Mobile** - Use phone camera to scan QR code
4. **View in AR** - Tap "View in AR" to place couch in your space

## Browser Support

### Desktop

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Mobile AR

- iOS 12+ (Safari with ARKit)
- Android 8+ (Chrome with ARCore)

## Performance

- **Optimized 3D Model** - Efficient GLB format
- **Texture Compression** - Optimized texture sizes
- **CDN Delivery** - Fast global content delivery
- **Caching** - Aggressive caching for static assets

## Customization

### Adding New Materials

1. Add texture files to appropriate folders
2. Update `FABRIC_OPTIONS` or `LEG_OPTIONS` arrays
3. Follow PBR texture naming conventions

### Model Replacement

1. Replace `couch.glb` with your model
2. Ensure mesh names follow conventions (Body, Plane, Stitch, Legs)
3. Test material assignments

## License

MIT License - Feel free to use and modify for your projects.
