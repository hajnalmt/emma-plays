# emma-plays Roadmap

This roadmap outlines the planned games and features for the emma-plays project. Each game is designed to teach specific concepts while keeping learning fun and engaging for children ages 4-10.

## Version Status

### Current Release

#### v0.1.0 - Kaleidoscope Creator ✅
**Status:** Released (2026-01-17)

A symmetrical drawing game that introduces mathematical concepts through creative play.

**Features:**
- Three symmetry modes (4-way, 6-way, 8-way)
- Ten vibrant colors
- Three brush sizes
- Save artwork as PNG
- Touch-optimized interface

**Educational Value:**
- Rotational and reflective symmetry
- Pattern recognition
- Color theory basics
- Fine motor skills
- Creative expression

---

## Planned Games

### v0.2.0 - Number Butterfly Garden 🦋

**Target Age:** 4-7 years

**Educational Skills:**
- Counting (1-20)
- Number recognition
- Even and odd numbers
- Skip counting (by 2s, 5s, 10s)
- One-to-one correspondence

**Game Concept:**
Numbers transform into colorful butterflies when clicked or tapped. Different numbers create different butterfly colors and patterns. Children can "plant" number flowers and watch their garden grow with mathematical beauty.

**Core Mechanics:**
- Click/tap numbers to spawn butterflies
- Even numbers = one color family, odd numbers = another
- Counting modes: Count by 1s, 2s, 5s, or 10s
- Butterflies flutter with CSS/SVG animations
- Garden fills with collected butterflies
- Reset to start a new garden

**Technical Approach:**
- SVG butterflies with CSS animations
- Click/tap event handlers
- Dynamic number generation
- Color palettes based on number properties
- Particle system for butterfly flight paths
- LocalStorage for saving favorite gardens (optional)

**Effort Estimate:** Medium
- Development: ~8-12 hours
- Testing: ~4 hours
- Documentation: ~2 hours

---

### v0.3.0 - Shape Pattern Builder 🔷

**Target Age:** 5-8 years

**Educational Skills:**
- Pattern recognition (AB, ABB, ABC, AABB)
- Logical reasoning
- Shape identification (circle, square, triangle, hexagon)
- Sequencing
- Prediction

**Game Concept:**
Children drag and drop shapes to complete or create patterns. The game provides pattern challenges (complete the pattern) and a free-build mode (create your own pattern). Completed patterns animate with celebration effects.

**Core Mechanics:**
- Drag-and-drop interface for shapes
- Multiple shape types and colors
- Pattern challenge mode (fill in the blank)
- Free-build creativity mode
- Pattern validation and feedback
- Celebration animations for correct patterns
- Increasing difficulty levels

**Technical Approach:**
- Drag-and-drop with touch support (Pointer Events API)
- Shape rendering with CSS or SVG
- Pattern validation algorithm
- Progressive difficulty system
- Sound effects for feedback (optional, with mute)
- Pattern generator for challenges

**Effort Estimate:** Medium-High
- Development: ~12-16 hours
- Testing: ~6 hours
- Documentation: ~3 hours

---

### v0.4.0 - Rainbow Spiral Drawer 🌀

**Target Age:** 6-10 years

**Educational Skills:**
- Mathematical spirals (Archimedean, Fibonacci)
- Geometry and curves
- Golden ratio introduction
- Angle and rotation concepts
- Parametric equations (visual understanding)

**Game Concept:**
An interactive drawing tool that creates beautiful mathematical spirals. Children control parameters like speed, tightness, and color transitions to see how mathematics creates natural patterns. Includes preset spirals (shells, galaxies, flowers) and custom creation mode.

**Core Mechanics:**
- Real-time spiral drawing with mouse/finger movement
- Preset spiral types (Fibonacci, Archimedean, logarithmic)
- Parameter controls (spacing, rotation, growth rate)
- Rainbow color transitions
- Speed control (fast/slow drawing)
- Save spirals as images
- Gallery of famous spirals in nature

**Technical Approach:**
- HTML5 Canvas for rendering
- Parametric equations for spiral generation
  - Archimedean: r = a + b×θ
  - Fibonacci/Golden: r = φ^(θ/90°)
- requestAnimationFrame for smooth animation
- HSL color space for rainbow gradients
- Interactive parameter sliders
- Mathematical visualization

**Effort Estimate:** High
- Development: ~16-20 hours
- Testing: ~6 hours
- Documentation: ~4 hours

---

### v0.5.0 - Music Pattern Maker 🎵

**Target Age:** 5-9 years

**Educational Skills:**
- Rhythm and timing
- Pattern sequences in music
- Auditory pattern recognition
- Cause and effect
- Creative composition

**Game Concept:**
A visual beat sequencer where children create rhythmic patterns using colored blocks. Each color represents a different instrument or sound. Patterns loop and can be layered to create simple songs. Teaches musical concepts through play.

**Core Mechanics:**
- Grid-based sequencer (8×8 or 16×8)
- Multiple instrument tracks (drums, piano, xylophone, etc.)
- Place/remove sounds by clicking/tapping
- Play/pause/stop controls
- Loop playback
- Save and load patterns
- Preset pattern library (copy and modify)
- Visual metronome

**Technical Approach:**
- Web Audio API for sound generation
- Synthesized sounds (no audio files needed for small size)
- Visual grid with CSS Grid
- Timing engine with precise scheduling
- Pattern data structure (2D array)
- Animation synced to playback
- Volume and tempo controls

**Effort Estimate:** High
- Development: ~20-24 hours
- Testing: ~8 hours
- Documentation: ~4 hours

---

## Community Ideas

We welcome game suggestions from the community! To propose a new game:

1. Open an issue with the "game-idea" label
2. Describe the concept and educational value
3. Suggest target age range
4. Include mockups or sketches if available

**Potential future game categories:**
- Math: Addition/subtraction puzzles, fraction visualizers
- Science: Simple physics simulations, weather patterns
- Language: Rhyming games, story builders (multilingual)
- Geography: Interactive maps, flag matching
- Time: Clock reading, calendar concepts

---

## Long-term Vision

### Progressive Web App (PWA)
**Effort:** High

Convert emma-plays into an installable PWA:
- Add manifest.json for installability
- Service worker for offline functionality
- Install prompt for home screen
- Works fully offline after first visit
- Native app-like experience on mobile

### Multilingual Support
**Effort:** Medium-High

Add language support starting with:
- Hungarian (native language for Emma)
- English (international reach)
- Icon-based UI minimizes text to translate
- Language selector in main catalog
- Per-game text translation files

### Accessibility Improvements
**Effort:** Medium

Enhance accessibility for all children:
- ARIA labels for screen readers
- Keyboard navigation support
- High contrast mode
- Reduce motion option
- Text-to-speech for instructions
- Colorblind-friendly palettes

### Performance Optimizations
**Effort:** Low-Medium

Improve load times and responsiveness:
- Image optimization and compression
- Lazy loading for games catalog
- Code minification (while keeping source readable)
- Progressive enhancement approach
- Lighthouse score optimization

### Educational Worksheets
**Effort:** Medium

Printable companion worksheets:
- PDF worksheets to complement games
- Offline activities related to concepts
- Parent/teacher guides
- Suggested discussion questions

### Teacher/Parent Dashboard
**Effort:** High

Optional tracking for educational settings:
- Progress tracking (opt-in, local only)
- Time spent per game
- Skills practiced
- Recommendations for next games
- Privacy-first approach (no cloud storage)

---

## Contributing to the Roadmap

Have ideas for new games or features? See our [Contributing Guidelines](CONTRIBUTING.md) for how to propose additions to this roadmap.

**Considerations for proposals:**
- Educational value must be clear
- Age-appropriateness (4-10 years)
- Technical feasibility with our no-dependency approach
- Privacy and safety for children
- Alignment with project philosophy

---

## Version Numbering

We follow [Semantic Versioning](https://semver.org/):
- **Major version (1.0.0):** Significant milestone (stable collection of 5+ games)
- **Minor version (0.x.0):** New game or major feature
- **Patch version (0.0.x):** Bug fixes, small improvements

Current status: Pre-release (0.x.x) until we reach a stable collection.

---

**Note:** This roadmap is aspirational and may change based on community feedback, available time, and emerging educational needs. All timelines are estimates and not commitments.

Built with ❤️ for Emma and all curious kids.
