# Particle Background

A lightweight JavaScript library that creates an animated particle background effect on an HTML canvas element.

## Features

- Smooth particle animations
- Responsive canvas sizing
- Customizable particle count
- Random particle colors and movements
- Easy to integrate

## Installation

1. Clone the repository or download the files
2. Include the `particleBackground.js` in your project

## Usage

```javascript
import { ParticleBackground } from './particleBackground.js';

// Initialize the background
const background = new ParticleBackground('your-canvas-id');
background.init(100); // Set number of particles
background.start();   // Start animation

// Stop animation if needed
background.stop();
```

## HTML Setup

```html
<canvas id="your-canvas-id"></canvas>
```

## Styling

Add this CSS to position your canvas:

```css
#your-canvas-id {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: -1;
}
```

## Customization

You can customize the particle behavior by modifying:

- Particle count: `background.init(numberOfParticles)`
- Particle size: Modify `size` in Particle class
- Particle speed: Adjust `vx` and `vy` calculations
- Colors: Update `generateColor()` method

## License

MIT License

## Contributing

Feel free to open issues and submit pull requests.
