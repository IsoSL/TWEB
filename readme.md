# Twitch Gaming Stream Website

A responsive website for your Twitch streaming channel focused on Call of Duty: Black Ops 6 and Rocket League.

## Features

- Responsive design that works on all devices
- Modern blue gaming theme
- Live Twitch stream embed
- Dynamic navigation with smooth scrolling
- Sections for your games, streaming schedule, and personal info
- Social media integration
- Mobile-friendly navigation

## Setup Instructions

### 1. Files Structure

This website consists of three main files:
- `index.html` - The main HTML structure
- `style.css` - All styling and design
- `script.js` - JavaScript functionality

### 2. Twitch Embed Setup

To make the Twitch embed work correctly:

1. In `script.js`, find the following code section:
```javascript
const options = {
    width: '100%',
    height: '100%',
    channel: 'YOUR_CHANNEL',
    parent: ['embed.example.com', 'localhost']
};
```

2. Replace `'YOUR_CHANNEL'` with your actual Twitch username
3. Update the `parent` array with your domain name once you deploy the website

### 3. Personalization

#### Profile Photo

To add your profile photo:
1. Replace the placeholder in the About section with your actual image:
```html
<div class="profile-placeholder">
    <i class="fas fa-user"></i>
</div>
```
2. Replace with:
```html
<img src="path/to/your-image.jpg" alt="Your Name">
```
3. Style it in CSS:
```css
.about-image img {
    width: 250px;
    height: 250px;
    border-radius: 50%;
    object-fit: cover;
    box-shadow: 0 10px 30px rgba(3, 169, 244, 0.4);
    border: 5px solid rgba(255, 255, 255, 0.1);
}
```

#### Game Images

Replace the placeholder game images:
1. Find the CSS classes `.bo6-card .game-image` and `.rl-card .game-image`
2. Replace the background URLs with paths to your actual game images

#### Text Content

1. Update the GamerTag in the header with your actual username
2. Customize schedule days and times to match your actual streaming schedule
3. Edit the About Me section with your personal gaming background
4. Update the Gaming Setup specifications with your actual hardware

#### Social Media Links

In the footer section, update the social media links with your actual profiles:
```html
<ul class="social-icons">
    <li><a href="https://twitch.tv/YOUR_USERNAME" target="_blank"><i class="fab fa-twitch"></i></a></li>
    <!-- Update other social links -->
</ul>
```

### 4. Deployment

1. Upload all three files to your web hosting provider
2. Make sure all files are in the same directory
3. Update the Twitch embed parent domains with your actual domain
4. Test the website on different devices to ensure it's working correctly

## Further Customization

### Color Scheme

If you want to modify the blue color scheme, edit the CSS variables at the top of the `style.css` file:

```css
:root {
    --primary-color: #1a73e8;
    --secondary-color: #0d47a1;
    --accent-color: #03a9f4;
    /* other color variables */
}
```

### Background Images

To change the background images:
1. Prepare high-quality images (1920x1080px or larger)
2. Upload them to your server
3. Update the background-image URLs in the CSS

## Browser Compatibility

This website is compatible with:
- Chrome 60+
- Firefox 60+
- Safari 12+
- Edge 79+
- Opera 47+

## Need Help?

If you need assistance with the setup or want to customize the website further, feel free to contact a web developer or reach out for support.
