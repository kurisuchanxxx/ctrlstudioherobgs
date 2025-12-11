# Liquid Ether Background

Full-screen fluid simulation background with interactive mouse effects for Webflow iframe embedding.

## Features

- Fluid dynamics simulation using WebGL
- Interactive mouse/touch interaction
- Auto-demo mode when idle
- Customizable color palette
- Performance optimized with IntersectionObserver

## Development

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Customization

Edit the default parameters in [src/App.jsx](src/App.jsx):

```jsx
<LiquidEther
  mouseForce={20}
  cursorSize={100}
  colors={['#5227FF', '#FF9FFC', '#B19EEF']}
  autoDemo={true}
  autoSpeed={0.5}
/>
```

### Available Props

- `mouseForce`: Strength of mouse interaction (default: 20)
- `cursorSize`: Size of interaction area (default: 100)
- `colors`: Array of hex colors for the fluid gradient
- `autoDemo`: Enable auto-animation when idle (default: true)
- `autoSpeed`: Speed of auto-animation (default: 0.5)
- `resolution`: Simulation resolution (default: 0.5)
- `isViscous`: Enable viscosity simulation (default: false)
- `BFECC`: Use BFECC advection for smoother results (default: true)

## Performance

The component automatically pauses rendering when not visible using IntersectionObserver.
