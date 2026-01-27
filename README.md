# Proto - Figma to HTML Screens

Pixel-perfect HTML screens that scale proportionally across all device sizes.

## Design Specifications

- **Base Design**: 360 × 800 pixels
- **Scaling**: Viewport-based proportional scaling
- **No breakpoints**: Single design that scales fluidly

## Project Structure

```
/Proto
├── index.html              # Main entry point
├── styles/
│   ├── base.css            # Reset, variables, scaling system
│   └── screens/            # Individual screen stylesheets
├── screens/                # HTML partials for each screen
├── assets/
│   ├── images/             # Exported Figma assets
│   └── fonts/              # Custom fonts
└── README.md
```

## Scaling System

The CSS uses viewport units to scale all measurements proportionally:

```css
/* All measurements use the --px variable */
.element {
  width: calc(100 * var(--px));      /* 100px at 360px viewport, scales up/down */
  font-size: calc(16 * var(--px));   /* 16px at 360px viewport, scales up/down */
}
```

## Running Locally

Simply open `index.html` in a browser, or use a local server:

```bash
# Using Python
python -m http.server 8000

# Using Node.js
npx serve
```

## Screens

| Screen | File | Status |
|--------|------|--------|
| TBD | - | Pending |

