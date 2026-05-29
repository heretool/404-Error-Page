# Cosmic 404 Error Page
A visually stunning, interactive 404 error page with a black hole/space theme featuring particle animations, mouse/touch interaction, and a "space warp" effect to return home.

<div align="center">
  <img src="https://github.com/heretool/404-Error-Page/blob/main/img.jpg" width="700">
</div>

## Features
- Real-time canvas-based black hole animation with particle accretion disk
- Mouse/touch tracking (black hole follows cursor with easing)
- Gravitational redshift color effects on particles
- Interactive "Initiate Space Warp" button with smooth fade-out transition
- Responsive design (works on mobile/desktop)
- Cosmic-themed UI with 3D text perspective and glow effects
- Open Graph meta tags for social sharing
- Smooth resize handling

## Demo
To see the page in action:
1. Clone this repository
2. Open `404.html` in a modern web browser
3. Hover/move your cursor to interact with the black hole
4. Click "Initiate Space Warp" to trigger the warp effect and return to the home page (replace `/` in the code with your actual home URL)

## Installation
1. Upload the entire file structure to your web server/GitHub Pages repository
2. Configure your web server to use `404.html` as the custom 404 error page:
   - For GitHub Pages: Place `404.html` in the root of your repository (GitHub automatically uses it as the 404 page)
   - For Apache: Add `ErrorDocument 404 /404.html` to your `.htaccess` file
   - For Nginx: Add `error_page 404 /404.html;` to your server configuration

## Customization
### Basic Customization
- **Text/Content**: Modify the `error-code`, `error-msg`, and button text in the HTML
- **Colors**: Adjust the hex/rgba values in the inline CSS (black hole glow, button colors, background)
- **Animation**: Tweak values like `maxParticles`, `blackHole.radius`, `gravity`, and `warpProgress` in the JavaScript
- **Home URL**: Change `window.location.href = '/'` (in the `animate()` function) to your actual home page URL

### Advanced Customization
- Adjust particle count (maxParticles) for performance (lower = faster on mobile)
- Modify black hole gravity/acceleration values
- Change the warp speed (warpProgress increment value)
- Update the Open Graph meta tags (title, description, image) to match your brand

## Browser Support
- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Mobile Safari/Chrome (responsive support)

## Performance Notes
- The canvas animation uses requestAnimationFrame for optimal performance
- Particle count is capped at 1400 (reduce for older devices)
- Touch interactions are passive to prevent scrolling issues on mobile

## License
This project is originally created and released by [heretool.com](https://heretool.com). It is open source and available under the [MIT License](https://opensource.org/licenses/MIT). Feel free to modify and use it for personal/commercial projects.
