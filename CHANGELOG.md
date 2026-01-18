# Changelog

All notable changes to emma-plays will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Planned
- Number Butterfly Garden game (v0.2.0)
- Shape Pattern Builder game (v0.3.0)
- Rainbow Spiral Drawer game (v0.4.0)
- Music Pattern Maker game (v0.5.0)
- GitHub Pages deployment
- Progressive Web App (PWA) support

## [0.1.0] - 2026-01-17

### Added

#### Project Infrastructure
- Initial project structure and repository setup at https://github.com/hajnalmt/emma-plays
- MIT License for open source sharing
- `.gitignore` for development environment files
- Comprehensive `README.md` with project philosophy, features, and educational value
- `CONTRIBUTING.md` with contribution guidelines and game design principles
- `ROADMAP.md` with future game plans and effort estimates
- Planning documentation structure in `planning/sessions/0001-emma-plays-initial-setup/`

#### Games Catalog
- Main `index.html` games catalog page with responsive grid design
- Beautiful gradient backgrounds and animations
- Game card previews with hover effects
- "Coming Soon" placeholders for future games
- Mobile-responsive layout (desktop and tablet optimized)

#### Kaleidoscope Creator Game
First playable game focused on symmetry and creative expression.

**Features:**
- Three symmetry modes: 4-way, 6-way, and 8-way rotational symmetry
- Ten vibrant colors: red, orange, yellow, green, cyan, blue, purple, pink, black, white
- Three brush sizes: small (5px), medium (15px), large (30px)
- Save artwork as PNG with timestamped filename (`kaleidoscope-{timestamp}.png`)
- Clear canvas function to start fresh
- Touch-screen optimized with dedicated touch event handlers
- Real-time symmetrical drawing with mirroring effect
- Smooth brush strokes using HTML5 Canvas with anti-aliasing
- Responsive design adapting to various screen sizes

**Technical Implementation:**
- HTML5 Canvas API for all drawing operations
- Pure JavaScript event handling (mouse and touch events)
- Mathematical symmetry calculation using rotation transforms
- Canvas state management (save/restore) for each symmetry segment
- Dynamic canvas sizing based on viewport (max 800×800px)
- Self-contained single HTML file (~13KB)

**User Interface:**
- Fixed control panel with semi-transparent background
- Large, tappable buttons (50-70px) optimized for children
- Icon-based controls (minimal text for pre-readers)
- Visual feedback on all interactions (hover states, active states)
- Color selection with active border indicator
- Symmetry mode selector with visual symbols (✚, ✱, ✻)
- Brush size selector with visual dot indicators

### Technical Details

#### Architecture
- Pure HTML/CSS/JavaScript (no frameworks or dependencies)
- Zero external libraries or npm packages
- Self-contained games (single file or simple folder structure)
- Works completely offline after initial load
- No build process required

#### Browser Support
- Modern browsers: Chrome, Firefox, Safari, Edge
- Desktop and mobile device support
- Touch and mouse event compatibility
- Responsive viewport handling

#### Performance
- Fast load times (<1 second for games)
- Efficient canvas rendering
- Minimal DOM manipulation
- Optimized for tablets and mobile devices

### Project Philosophy

This release establishes the core principles of emma-plays:

- **Kid-safe:** No ads, tracking, external links, or data collection
- **Educational focus:** Every game teaches mathematical concepts, patterns, or creativity
- **Touch-friendly:** Large buttons (50-70px minimum), optimized for tablets and young fingers
- **Minimal text:** Icon-based UI suitable for pre-readers and multilingual use
- **Accessibility:** High contrast colors, visual feedback, intuitive interactions
- **Privacy-first:** No analytics, no cookies, no personal data collection
- **Open source:** MIT License encourages sharing, remixing, and learning from code

### Educational Value

#### Kaleidoscope Creator teaches:
- **Rotational symmetry:** Understanding how objects look the same after rotation
- **Reflective symmetry:** Understanding mirror images
- **Pattern recognition:** Observing repeated elements
- **Cause and effect:** Drawing actions create immediate visual results
- **Color theory basics:** Exploring color combinations
- **Fine motor skills:** Precise finger/mouse control
- **Creative expression:** Freedom to create without "wrong" answers
- **Mathematical art:** Beauty in mathematical patterns

### Repository Structure

```
emma-plays/
├── .git/                    # Git repository metadata
├── .gitignore              # Ignored files (130 bytes)
├── LICENSE                 # MIT License (1,070 bytes)
├── README.md               # Project overview (3,886 bytes)
├── CONTRIBUTING.md         # Contribution guidelines
├── ROADMAP.md             # Future plans
├── CHANGELOG.md           # This file
├── index.html              # Games catalog (9,496 bytes)
├── kaleidoscope/
│   └── index.html          # Kaleidoscope game (13,000 bytes)
└── planning/
    └── sessions/
        └── 0001-emma-plays-initial-setup/
            ├── PLAN.md     # Session planning document
            └── SUMMARY.md  # Session summary
```

### Statistics

- **Repository Size:** ~42KB (minimal, fast loading)
- **Lines of Code:** ~950 lines (excluding documentation)
- **Documentation:** ~1,200 lines
- **Games Playable:** 1
- **Games Planned:** 4
- **Target Age Range:** 4-10 years
- **Supported Languages:** English (UI mostly icon-based)

### Credits

- **Created by:** Hajnal Máté
- **Inspired by:** Emma, a curious 5-year-old who loves patterns and colors
- **License:** MIT License
- **Repository:** https://github.com/hajnalmt/emma-plays

---

## Version History Links

[Unreleased]: https://github.com/hajnalmt/emma-plays/compare/v0.1.0...HEAD
[0.1.0]: https://github.com/hajnalmt/emma-plays/releases/tag/v0.1.0

---

**Note:** This changelog will be updated with each release. For detailed development session notes, see the `planning/sessions/` directory.
