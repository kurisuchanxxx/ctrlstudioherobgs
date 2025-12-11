# CTRL Studio Hero Backgrounds

Collection of animated hero backgrounds for Webflow integration via iframe.

## Available Backgrounds

### [Dither](./dither)
Full-screen animated dither effect with mouse interaction.

- **Demo**: [Live on Vercel](https://ctrlstudioherobgs.vercel.app)
- **Tech**: React, Three.js, WebGL shaders, @react-three/fiber
- **Features**: Animated waves, dithering effect, mouse interaction

### [Liquid Ether](./liquid-ether)
Fluid dynamics simulation with interactive mouse effects.

- **Demo**: [Live on Vercel](https://ctrlstudioherobgs.vercel.app)
- **Tech**: React, Three.js, WebGL fluid simulation
- **Features**: Fluid dynamics, customizable colors, auto-demo mode, touch support

## Development

Each background is a separate Vite project. Navigate to the specific folder:

```bash
cd dither
npm install
npm run dev
```

## Deployment

Each background can be deployed separately on Vercel or as part of this monorepo.

### Deploy individual backgrounds:
1. Each folder is a standalone Vite project
2. Can be deployed to separate Vercel projects

### Deploy as monorepo:
Vercel will auto-detect each subfolder as a separate project.

## Webflow Integration

Use iframe embedding in Webflow:

```html
<iframe
  src="https://YOUR-PROJECT.vercel.app/dither"
  style="width: 100%; height: 100%; border: none;"
  loading="lazy"
></iframe>
```

## Structure

```
ctrlstudioherobgs/
├── dither/          # Dither effect background
│   ├── src/
│   ├── package.json
│   └── vite.config.js
├── liquid-ether/    # Fluid simulation background
│   ├── src/
│   ├── package.json
│   └── vite.config.js
└── [future-backgrounds]/
```

## Adding New Backgrounds

1. Create a new folder with a Vite React project
2. Update this README
3. Add deployment configuration if needed
