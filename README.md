# Bits N Pieces - Coming Soon Landing Page

A beautiful, minimal yet creative coming soon landing page for your thrift store with email subscription functionality.

## Features

- ✨ **Minimal & Creative Design**: Clean, modern aesthetic with subtle animations
- 🔘 **Rounded Buttons**: Beautiful rounded UI elements throughout
- 📧 **Email Subscription**: Functional email collection form with validation
- 📱 **Responsive Design**: Works perfectly on all devices
- 🎨 **Smooth Animations**: Subtle hover effects and entrance animations
- 🌟 **Floating Elements**: Creative background elements that add personality
- 💾 **Local Storage**: Stores subscriber emails locally (can be connected to backend)

## Files

- `index.html` - Main HTML structure
- `styles.css` - All styling and animations
- `script.js` - JavaScript functionality and form handling
- `README.md` - This file

## How to Use

1. **Open the page**: Simply open `index.html` in any modern web browser
2. **Customize content**: Edit the text, colors, and branding in the HTML and CSS files
3. **Deploy**: Upload all files to your web hosting service

## Customization

### Changing Colors
The main color scheme uses CSS custom properties. You can modify the gradients in `styles.css`:

```css
/* Primary gradient for buttons and logo */
background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);

/* Background gradient */
background: linear-gradient(135deg, #f5f7fa 0%, #c3cfe2 100%);
```

### Changing Text
Edit the content in `index.html`:
- Store name: Change "Bits N Pieces" to your store name
- Tagline: Modify the description and features
- Contact information: Update any contact details

### Adding Backend Integration
To connect the email subscription to a real backend:

1. Replace the setTimeout in `script.js` with an actual API call
2. Add your backend endpoint URL
3. Handle success/error responses from your server

Example:
```javascript
// Replace the setTimeout with:
fetch('/api/subscribe', {
    method: 'POST',
    headers: { 'Content-Type': 'application/json' },
    body: JSON.stringify({ email: email })
})
.then(response => response.json())
.then(data => {
    showMessage('Thank you for subscribing!', 'success');
    emailInput.value = '';
})
.catch(error => {
    showMessage('Something went wrong. Please try again.', 'error');
});
```

## Browser Support

- Chrome (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)

## License

Feel free to use and modify this landing page for your business needs.

## Support

If you need help customizing or have questions, feel free to reach out!
