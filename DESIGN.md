---
name: Cyber-Terminal Industrial
colors:
  surface: '#131313'
  surface-dim: '#131313'
  surface-bright: '#3a3939'
  surface-container-lowest: '#0e0e0e'
  surface-container-low: '#1c1b1b'
  surface-container: '#201f1f'
  surface-container-high: '#2a2a2a'
  surface-container-highest: '#353534'
  on-surface: '#e5e2e1'
  on-surface-variant: '#b9cac4'
  inverse-surface: '#e5e2e1'
  inverse-on-surface: '#313030'
  outline: '#83948f'
  outline-variant: '#3a4a46'
  surface-tint: '#00dfc1'
  primary: '#d7fff3'
  on-primary: '#00382f'
  primary-container: '#00f5d4'
  on-primary-container: '#006c5c'
  inverse-primary: '#006b5b'
  secondary: '#c6c7c6'
  on-secondary: '#2f3131'
  secondary-container: '#454747'
  on-secondary-container: '#b4b5b5'
  tertiary: '#fff5e4'
  on-tertiary: '#3c2f00'
  tertiary-container: '#ffd651'
  on-tertiary-container: '#745c00'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#26fedc'
  primary-fixed-dim: '#00dfc1'
  on-primary-fixed: '#00201a'
  on-primary-fixed-variant: '#005144'
  secondary-fixed: '#e2e2e2'
  secondary-fixed-dim: '#c6c7c6'
  on-secondary-fixed: '#1a1c1c'
  on-secondary-fixed-variant: '#454747'
  tertiary-fixed: '#ffe086'
  tertiary-fixed-dim: '#eac33f'
  on-tertiary-fixed: '#231b00'
  on-tertiary-fixed-variant: '#574500'
  background: '#131313'
  on-background: '#e5e2e1'
  surface-variant: '#353534'
typography:
  display-xl:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: '1.1'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.6'
  mono-label:
    fontFamily: Space Grotesk
    fontSize: 14px
    fontWeight: '500'
    lineHeight: '1.0'
    letterSpacing: 0.1em
  caption-mono:
    fontFamily: Space Grotesk
    fontSize: 10px
    fontWeight: '400'
    letterSpacing: 0.05em
spacing:
  xs: 4px
  sm: 8px
  md: 16px
  lg: 32px
  xl: 64px
  section: 128px
  container-max: 1280px
---

## Brand & Style
The brand identity is rooted in high-performance computing, AI automation, and technical precision. It evokes the feeling of a "Command Center" or a developer's terminal, emphasizing reliability, speed, and vertical scaling. 

The design style is a hybrid of **Cyber-Brutalism** and **Terminal Aesthetics**. It features sharp edges, monospaced data readouts, and high-contrast "neon" accents against deep obsidian backgrounds. The emotional response is one of specialized expertise—functional, futuristic, and unyielding. Visual interest is driven by technical artifacts: scanlines, grain overlays, animated grid lines, and glowing data points that suggest a living, breathing system rather than a static page.

## Colors
The palette is dominated by "Pure Obsidian" and "Deep Charcoal" to create a void-like backdrop that mimics a dark-mode IDE. 

- **Primary (Electric Cyan):** Used exclusively for interactive elements, status indicators, and data-core visualizations. It carries a glow effect to simulate light emission from a screen.
- **Secondary (Muted Steel):** Used for auxiliary data paths and non-critical structural elements.
- **Background Details:** The background is not a flat hex; it uses a subtle 32px radial dot grid (`#1a1a1a`) and a 3% opacity film grain overlay to add tactile texture to the digital space.
- **Text:** Primary information uses a high-contrast off-white, while metadata and labels use a muted teal-grey to maintain hierarchy.

## Typography
The typographic system relies on the tension between the technical, geometric nature of **Space Grotesk** and the utilitarian clarity of **Inter**.

- **Headlines:** Use Space Grotesk with tight letter spacing for a compact, engineered look.
- **Body:** Inter provides maximum readability for technical descriptions and documentation.
- **System Labels:** Small-caps or all-caps monospaced-style Space Grotesk is used for "system logs," status codes, and button labels to reinforce the terminal theme. 
- **Interactive States:** Use a custom blinking cursor (`12px x 24px` block) at the end of display headings to simulate an active command line.

## Layout & Spacing
The system uses a **Fixed Grid** philosophy with generous vertical "safe zones" between major sections (128px). 

- **Grid:** A 12-column layout with 32px gutters.
- **Section Dividers:** Horizontal rules with centered system metadata (e.g., `--- production.log ---`) act as break points between logic blocks.
- **Alignment:** Content is generally left-aligned to mimic code structures, while hero sections and service headers utilize centered alignment for impact. 
- **Density:** High information density is encouraged within "Terminal Cards," but surrounded by significant whitespace to maintain a premium, architectural feel.

## Elevation & Depth
Depth is created through **Tonal Layering** and **Luminous Accents** rather than traditional shadows.

- **Base Layer:** The obsidian background with radial dot pattern.
- **Mid-Tier:** Terminal windows and cards use `#131313` with a sharp `1px` border in `#1c1b1b`.
- **Top-Tier (Active):** Elements in focus or hovered receive a `terminal-glow` effect: a primary-colored outer glow (`0 0 15px rgba(0, 245, 212, 0.3)`) and a border-color shift to the Primary Cyan.
- **Overlays:** A grain overlay is fixed to the viewport at a very low opacity, acting as a "screen texture" that sits above all UI elements.

## Shapes
The shape language is strictly **Sharp (0px)**. This reinforces the brutalist, industrial nature of the system. 

- **Exceptions:** Circular geometry is reserved strictly for "living" data visualizations (e.g., the spinning data core, orbit rings, and status pips) to create a contrast between the rigid structural containers and the fluid AI logic they house. 
- **Buttons & Inputs:** Must always have 0px border-radius, maintaining a modular, brick-like appearance.

## Components
- **Primary Button:** Solid Primary Cyan background, black text. High-contrast, no rounding. On hover, it gains a Cyan drop-shadow/glow.
- **Secondary Button:** Outlined with Primary Cyan, transparent background. 10% Cyan fill on hover.
- **Terminal Cards:** Dark grey containers with a dedicated header bar containing "Window Controls" (three neutral pips) and a monospaced filename/label.
- **Data Tags/Chips:** Tiny, outlined boxes with Space Grotesk text. Used for tech stacks (e.g., "PYTHON," "LLMs").
- **Input Fields:** Obsidian background, thin neutral border that glows Primary Cyan on focus. Labels sit above the field in a muted, uppercase mono-font.
- **Visualizers:** Use SVG-based lines with `stroke-dasharray` animations to represent data flow and "live" system processing.