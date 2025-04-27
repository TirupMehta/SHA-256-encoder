# SHA-256: Hash Generator

## Description

**SHA-256** is a minimalist, futuristic hash generator that transforms your text into a SHA-256 hash with a single click.  
Encased in a dark, glassmorphic interface, it pulses with subtle particle effects and a custom cursor, drawing you into a shadowy digital realm.

The tool fetches your input, generates a secure hash, and lets you copy it to the clipboard with a toast notification.  
Red particles flare briefly during hashing, a nod to the beating heart of code.

> "Encrypt your story, leave no trace."

---

## Overview

CipherHeart is a web-based SHA-256 hash generator designed with a dark, cyberpunk aesthetic.  
It features a custom cursor, an interactive particle background, and smooth animations, creating an immersive experience.  
Users can input text, generate a hash, and copy it to the clipboard, with visual feedback like pulsing red particles and toast notifications.  
It is ideal for developers, hobbyists, and anyone drawn to sleek, moody tools.

---

## Features

- **SHA-256 Hashing**: Generates secure hashes from user input using the Web Crypto API.
- **Interactive Design**: Custom cursor grows and shifts to red on hover, with particle effects that pulse during hashing.
- **Clipboard Support**: Copy generated hashes with a single click, confirmed by a toast notification.
- **Dark Romance Aesthetic**: Glassmorphic container, gradient text, and a cryptic tagline.
- **Responsive Layout**: Adapts to various screen sizes, with the custom cursor disabled on touch devices for performance.

---

## Installation

1. **Download**: Clone or download the `index.html` file from the repository.
2. **Host**: Serve the file using a local server (for example, `python -m http.server` or VS Code **Live Server**) or upload it to a web host.
3. **Dependencies**: No installation required; the tool uses CDN-hosted Particles.js and native browser APIs.

---

## Usage

1. Open `index.html` in a modern browser (Chrome, Firefox, or Edge recommended).
2. Enter text in the input field.
3. Click **"Generate SHA-256"** to create a hash, displayed below.
4. Click **"Copy Hash"** to copy the hash to your clipboard; a toast notification will confirm the action.
5. Observe the particles pulse red briefly during hashing for a visual effect.

---

## File Structure

- `index.html`: Contains all HTML, CSS, JavaScript, and logic for the tool.

External dependencies (loaded via CDN):
- [Particles.js](https://cdn.jsdelivr.net/npm/particles.js@2.0.0/particles.min.js)
- [Google Fonts (Inter)](https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap)

---

## Customization

- **Change Hash Algorithm**:  
  Modify the `crypto.subtle.digest` call inside the `generateHash` function to support different algorithms (such as SHA-1, SHA-512).

- **Adjust Aesthetics**:
  - Edit the `particlesJS` configuration within the `<script>` section to change particle color, speed, or shape.
  - Update CSS variables (such as those for `.cursor` and `.container`) to alter colors or effects.
  - Modify the tagline within the `<p>` element to suit your preferred narrative tone.

- **Extend Features**:
  - Support file hashing by processing uploaded files as ArrayBuffers.
  - Add multiple hash types via a dropdown menu.

---

## Technical Details

- **Tech Stack**: HTML5, CSS3, JavaScript (ES6), Web Crypto API, Particles.js
- **Browser Compatibility**: Compatible with modern browsers supporting Web Crypto API and CSS `backdrop-filter`.
- **Performance**: Optimized with `requestAnimationFrame` for smooth cursor animation and deferred loading of Particles.js for faster page load.
- **Accessibility**: Basic ARIA labels and keyboard support included. Focus states and screen reader improvements can be added.

---

## Limitations

- Requires an internet connection to load external resources (Particles.js and Google Fonts).
- Hashing is limited to SHA-256 by default; adding other algorithms requires manual changes.
- File input is not currently supported; the tool works only with text.
- The custom cursor is disabled on touch devices to improve usability.

---

## Future Enhancements

- Add support for multiple hash algorithms (MD5, SHA-1, SHA-512) through a selection dropdown.
- Implement file hashing by processing uploaded files.
- Create a settings panel to toggle particle effects and cursor styles.
- Improve accessibility with full keyboard navigation and enhanced screen reader compatibility.

---

## Contributing

Contributions are welcome.  
Feel free to fork the project and submit pull requests for new features, improvements, or bug fixes.  
Suggestions for expanding the narrative or adding cyberpunk-inspired enhancements are also appreciated.

---

## License

This project is licensed under the MIT License.  
You are free to use, modify, and distribute it, but keep the spirit of the project intact.

---

## Acknowledgments

- Inspired by the sleek, futuristic aesthetic of **CheckmateBegins**.
- Built with passion for those who find beauty in both code and darkness.
