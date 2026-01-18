# Contributing to emma-plays

Thank you for your interest in contributing to emma-plays! This project aims to create fun, educational, and safe games for young children (ages 4-10). We welcome contributions from developers, educators, parents, and anyone passionate about creating quality learning experiences for kids.

## Table of Contents

- [How to Contribute](#how-to-contribute)
- [Game Design Guidelines](#game-design-guidelines)
- [Code Style Guidelines](#code-style-guidelines)
- [Testing Your Contribution](#testing-your-contribution)
- [Submitting Pull Requests](#submitting-pull-requests)
- [Code of Conduct](#code-of-conduct)
- [Questions and Support](#questions-and-support)

## How to Contribute

### Reporting Issues

If you find a bug or have a suggestion:

1. Check if the issue already exists in the [Issues](https://github.com/hajnalmt/emma-plays/issues) section
2. If not, create a new issue with:
   - Clear, descriptive title
   - Detailed description of the problem or suggestion
   - Steps to reproduce (for bugs)
   - Screenshots or videos if applicable
   - Browser and device information (for bugs)

### Contributing Code

1. **Fork the repository** to your own GitHub account
2. **Clone your fork** to your local machine
   ```bash
   git clone https://github.com/YOUR-USERNAME/emma-plays.git
   cd emma-plays
   ```
3. **Create a new branch** for your feature or fix
   ```bash
   git checkout -b feature/your-game-name
   # or
   git checkout -b fix/bug-description
   ```
4. **Make your changes** following our guidelines (see below)
5. **Test thoroughly** on multiple devices and browsers
6. **Commit your changes** with clear, descriptive messages
   ```bash
   git commit -s -m "Add interactive math puzzle game"
   ```
7. **Push to your fork**
   ```bash
   git push origin feature/your-game-name
   ```
8. **Open a Pull Request** with a detailed description of your changes

## Game Design Guidelines

All games in emma-plays must follow these principles:

### Age-Appropriate Content (4-10 years)

- Simple, intuitive controls
- Large touch targets (minimum 50px, recommended 60-70px)
- Minimal text - use icons and visual cues
- Bright, engaging colors
- Clear visual feedback for all interactions
- No scary, violent, or inappropriate content

### Educational Value Required

Every game should teach or reinforce at least one concept:
- **Math:** Counting, patterns, shapes, symmetry, arithmetic
- **Logic:** Sequencing, problem-solving, cause-and-effect
- **Creativity:** Art, music, self-expression
- **Motor Skills:** Hand-eye coordination, fine motor control

Document the educational goals in your game's README or comments.

### Technical Requirements

#### No External Dependencies
- Pure HTML5, CSS3, and JavaScript (ES6+)
- No frameworks, libraries, or npm packages
- Self-contained single file or simple folder structure
- Must work offline once loaded

#### Browser Compatibility
- Support modern browsers: Chrome, Firefox, Safari, Edge
- Test on both desktop and mobile
- Use standard web APIs (avoid experimental features)

#### Touch and Mouse Compatible
- Support both touch events and mouse events
- Test on tablets and touchscreens
- Ensure buttons work well with fingers (not just mouse clicks)
- No hover-only interactions (touch devices can't hover)

#### Responsive Design
- Work on various screen sizes (phone, tablet, desktop)
- Use viewport meta tag
- Test in portrait and landscape orientations
- Maximum game size: 800-1000px for optimal performance

#### No Data Collection or Tracking
- No analytics or tracking scripts
- No cookies or local storage (unless essential for game functionality)
- No external API calls
- No third-party services
- Privacy is paramount for children's content

### User Interface Guidelines

- **Icon-based:** Use symbols and emojis rather than words when possible
- **High contrast:** Ensure text and icons are easily visible
- **Clear feedback:** Visual and/or audio response to all actions
- **Obvious controls:** No hidden or complex UI elements
- **Minimal chrome:** Focus on the game, not the interface
- **Save functionality:** Allow saving/downloading creations when applicable

## Code Style Guidelines

### HTML

- Use semantic HTML5 elements
- Include proper `<!DOCTYPE html>`
- Set viewport for mobile: `<meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">`
- Use meaningful IDs and classes
- Keep structure simple and readable

### CSS

- Embed styles in `<style>` tags for self-contained games
- Use modern CSS (Flexbox, Grid)
- Avoid overly complex selectors
- Include transitions for interactive feedback
- Use relative units (rem, %, vh/vw) for responsiveness
- Comment complex styling rules

### JavaScript

- Use modern ES6+ syntax
- Embed scripts in `<script>` tags (unless game is complex)
- Clear, descriptive variable and function names
- Comment complex logic
- Handle both touch and mouse events
- Prevent default touch behaviors when needed (`touch-action: none`)
- Clean up event listeners if dynamic
- Use `requestAnimationFrame` for animations
- Keep code readable - prioritize clarity over cleverness

### File Naming

- Game folders: lowercase with hyphens (e.g., `number-butterfly-garden/`)
- Main file: `index.html`
- Assets (if needed): organized in subfolders (`assets/images/`, `assets/sounds/`)

### Comments

Add educational comments explaining:
- What mathematical or educational concept is being demonstrated
- How algorithms work (especially complex ones)
- Why certain design decisions were made

This helps teachers and parents understand the learning value.

## Testing Your Contribution

Before submitting, test your game on:

### Browsers
- Chrome (desktop and mobile)
- Firefox
- Safari (iOS if possible)
- Edge

### Devices
- Desktop computer (various screen sizes)
- Tablet (iPad or Android)
- Smartphone (portrait and landscape)

### Testing Checklist
- [ ] All buttons are easily tappable with a finger
- [ ] Touch and mouse input both work
- [ ] Game works in portrait and landscape
- [ ] No console errors
- [ ] Responsive design works at different sizes
- [ ] Game loads quickly (< 2 seconds)
- [ ] Instructions are clear (or not needed)
- [ ] Educational value is apparent
- [ ] No inappropriate content
- [ ] Offline functionality works

## Submitting Pull Requests

### PR Title Format

Use clear, descriptive titles:
- `Add: Number Butterfly Garden game`
- `Fix: Touch input not working in Kaleidoscope`
- `Improve: Responsive design for Shape Pattern Builder`
- `Update: Documentation for contributing guidelines`

### PR Description

Include:
1. **What:** Brief description of changes
2. **Why:** Reason for the changes or problem being solved
3. **Educational Value:** What skills does the game teach (for new games)
4. **Testing:** How you tested the changes
5. **Screenshots:** Visual examples of the game (for new games or UI changes)
6. **Target Age:** Recommended age range (for new games)

### Review Process

1. Maintainer will review your PR
2. May request changes or improvements
3. Once approved, your contribution will be merged
4. You'll be credited in the commit and potentially in documentation

## Code of Conduct

This is a project for children. All contributors must:

- **Be respectful** in all interactions
- **Keep content child-appropriate** at all times
- **Prioritize safety and privacy** of young users
- **Welcome newcomers** and help them contribute
- **Focus on education and fun** as primary goals
- **Avoid controversial or divisive topics** - stick to universal learning concepts

Unacceptable behavior:
- Inappropriate content or language
- Harassment or discrimination
- Privacy violations
- Malicious code or security issues

Violations may result in removal from the project.

## Questions and Support

### Where to Ask

- **GitHub Issues:** Bug reports and feature requests
- **Pull Request Comments:** Questions about specific contributions
- **Discussions:** General questions and ideas (if enabled)

### Response Time

This is a volunteer project. Please be patient:
- Issues: Typically reviewed within 1 week
- Pull Requests: Typically reviewed within 2 weeks

### Getting Help

If you're stuck:
1. Check existing issues and pull requests
2. Review the [ROADMAP.md](ROADMAP.md) for planned features
3. Look at existing games for examples
4. Create an issue explaining what you need help with

---

## Thank You!

Every contribution, no matter how small, helps make learning more fun and accessible for children. Whether you're fixing a typo or building an entire game, your effort is appreciated!

Built with ❤️ for Emma and all curious kids.
