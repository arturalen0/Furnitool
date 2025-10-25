# 3D Couch Configurator

A professional 3D furniture configurator that allows users to customize couch materials and switch between different couch models.

## Features

- **Real-time 3D Configurator** - Interactive Three.js-powered 3D models
- **Model Selection** - Choose from 13 different couch models
- **Material Customization** - Choose from multiple fabric, stitch, and leg options
- **Professional Lighting** - Cinema-quality lighting with shadows and effects
- **Smooth Controls** - Professional camera controls with constraints
- **Dynamic Model Loading** - Switch between different couch models instantly

## Technology Stack

- **Three.js** - 3D rendering and controls
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

1. **Select Model** - Choose from 13 different couch models using the dropdown
2. **Configure Materials** - Select fabric, stitch color, and leg materials
3. **Real-time Preview** - See changes applied instantly to the 3D model
4. **Professional Controls** - Use mouse/trackpad to rotate, zoom, and pan

## Browser Support

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

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
