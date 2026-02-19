# GLM OS Test - Interactive OS Demos

A collection of interactive web-based operating system demos showcasing different OS interfaces and designs.

## Live Demos

- **Windows Demo**: [https://echooff3.github.io/glm-os-test/](https://echooff3.github.io/glm-os-test/)
- **Windows 8 Metro**: [https://echooff3.github.io/glm-os-test/metro.html](https://echooff3.github.io/glm-os-test/metro.html)
- **BeOS Demo**: [https://echooff3.github.io/glm-os-test/beos.html](https://echooff3.github.io/glm-os-test/beos.html)
- **iPhone OS Demo**: [https://echooff3.github.io/glm-os-test/iphone.html](https://echooff3.github.io/glm-os-test/iphone.html)
- **Android Marshmallow Demo**: [https://echooff3.github.io/glm-os-test/android.html](https://echooff3.github.io/glm-os-test/android.html)

## Features

### OS Navigation Icons

Each operating system demo now includes **desktop icons or tiles** that allow you to navigate between different OS demos:

- **Windows Demo** (`index.html`): Look for the **BeOS Demo**, **Windows 8 Metro**, **iPhone OS**, and **Android** icons in the top-right corner of the desktop
- **BeOS Demo** (`beos.html`): Look for the **Windows Demo**, **Windows 8 Metro**, **iPhone OS**, and **Android** icons in the top-right corner of the desktop
- **Windows 8 Metro** (`metro.html`): Scroll down to the **"Try Other OS Demos"** section with tiles for **Windows Demo**, **BeOS Demo**, **iPhone OS Demo**, and **Android Demo**
- **iPhone OS Demo** (`iphone.html`): Open the **OS Demos** app to find links to all other demos
- **Android Marshmallow Demo** (`android.html`): Open the **OS Demos** app to find links to all other demos

Simply **double-click** the desktop icons (Windows/BeOS) or **click** the tiles (Metro) to navigate between demos.

### Icon Design

Each OS navigation icon features:
- **Distinctive SVG graphics** representing each operating system
- **OS-appropriate styling** matching the host OS theme
- **Hover effects** for better user interaction
- **Resolution-independent** vector graphics for crisp display at any size

## Testing OS Icons

### Basic Navigation Test

1. Open any OS demo in your browser
2. Locate the OS navigation icons (top-right for Windows/BeOS, bottom section for Metro)
3. Double-click (desktop icons) or click (Metro tiles) to navigate to another OS demo
4. Verify smooth transition and proper loading of the target OS

### Resolution Compatibility Test

Open `icon-compatibility-test.html` to test icon rendering at different resolutions:
- Tests three standard resolutions: 1920×1080, 1366×768, and 1280×720
- Validates icon visibility and click responsiveness
- Checks hover effects and styling

### Browser Compatibility

Tested and working on:
- Chrome/Edge (Chromium-based browsers)
- Firefox
- Safari
- Opera

## Customizing OS Icons

### Changing Icon Appearance

Icons are defined using inline SVG within each demo file. To customize:

1. **Windows Demo** (`index.html`): Look for the `addOSNavigationIcons()` method in the Desktop class
2. **BeOS Demo** (`beos.html`): Look for the `addOSNavigationIcons()` method in the Desktop class
3. **Metro Demo** (`metro.html`): Look for the OS Demo tiles section with the "Try Other OS Demos" heading

### Adding New OS Demos

To add a new OS demo with navigation icons:

1. Create your new OS demo HTML file (e.g., `macos.html`)
2. Add navigation icons in the existing demos pointing to your new demo
3. Add navigation icons in your new demo pointing back to existing demos
4. Update this README with the new demo link

### Icon Styling

CSS classes for OS navigation icons:
- `.desktop-icon.os-link` - Base styling for desktop icons (Windows/BeOS)
- `.desktop-icon.os-link.beos` - BeOS-specific icon styling
- `.desktop-icon.os-link.metro` - Metro-specific icon styling
- `.desktop-icon.os-link.windows` - Windows-specific icon styling
- `.desktop-icon.os-link.android` - Android-specific icon styling
- `.os-demo-tile` - Metro tile styling for OS demos

## Contributing

Contributions are welcome! If you'd like to add features or improve existing demos:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test across different browsers and resolutions
5. Submit a pull request

## License

This project is open source and available for educational and demonstration purposes.
