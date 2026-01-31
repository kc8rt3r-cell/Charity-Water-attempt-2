# Website Editing Guide for Beginners

Welcome! This guide will help you customize your website without needing to know how to code.

## Quick Start

1. Open `index.html` in a text editor (like Notepad or VS Code)
2. Find the text you want to change
3. Edit it and save the file
4. Open `index.html` in your web browser to see the changes

### Permanent Preview Port (Recommended)
To keep your preview consistent, use a fixed local port whenever you edit:

1. Open a terminal in this project folder
2. Run this command:
   ```bash
   python3 -m http.server 4173
   ```
3. Open your browser to: `http://localhost:4173`

From now on, always use port **4173** for local previews so your workflow stays consistent.

---

## Editing the Text Content

### Page Title (Browser Tab)
In `index.html`, find this line near the top:
```html
<title>My Website</title>
```
Change `My Website` to whatever you want people to see in their browser tab.

### Header (Top of Page)
Find this section:
```html
<h1>Welcome to My Website</h1>
<p class="tagline">This is my tagline - change it to something meaningful!</p>
```
- Change `Welcome to My Website` to your main heading
- Change the tagline to your own tagline

### Menu Links
Find this section and change the text in the menu:
```html
<a href="#home" class="nav-link">Home</a>
<a href="#about" class="nav-link">About</a>
<a href="#services" class="nav-link">Services</a>
<a href="#contact" class="nav-link">Contact</a>
```
You can change "Home", "About", "Services", "Contact" to anything you'd like.

### Main Sections
Find each section like this:
```html
<section id="home" class="section">
    <h2>Welcome!</h2>
    <p>Your text here</p>
</section>
```
- Change the `<h2>` text to your section title
- Change the `<p>` text to your content
- You can add more `<p>` tags for more paragraphs

### Service Cards
Find this section:
```html
<div class="card">
    <h3>Service 1</h3>
    <p>Describe your first service or feature here.</p>
</div>
```
- Change "Service 1" to the name of what you offer
- Change the description
- Duplicate this `<div class="card">` block if you want more services

### Contact Information
Find this section:
```html
<p>
    <strong>Email:</strong> your.email@example.com<br>
    <strong>Phone:</strong> (555) 123-4567<br>
    <strong>Location:</strong> Your City, Your State
</p>
```
Replace with your actual contact information.

### Footer
Find this at the bottom:
```html
<p>&copy; 2026 My Website. All rights reserved.</p>
<p>Made with care for the web.</p>
```
Change the year and the footer text to whatever you'd like.

---

## Customizing Colors

Open `styles.css` and look for color values like this:
```css
background-color: #2c3e50;
color: white;
```

### Common Color Changes

**Header/Footer Background**: Find `.header` and `.footer` - change the `background-color`

**Text Color**: Find the section and change `color:`

**Card Background**: Find `.card` and change `background-color:`

### Using Color Names or Hex Codes
You can use:
- **Color names**: `white`, `black`, `blue`, `red`, `green`, `gray`, `yellow`, `orange`, `purple`
- **Hex codes**: `#2c3e50`, `#3498db`, `#e74c3c`, etc.

Find hex color codes at: https://htmlcolorcodes.com/

### Example Color Changes
Replace this:
```css
background-color: #2c3e50; /* Dark blue */
```

With this:
```css
background-color: #e74c3c; /* Red */
```

---

## Customizing Fonts

In `styles.css`, find this line:
```css
font-family: 'Arial', sans-serif;
```

Change `Arial` to:
- `Georgia` - elegant serif font
- `Courier New` - monospace font
- `Verdana` - clean sans-serif
- `Times New Roman` - classic serif

Example:
```css
font-family: 'Georgia', serif;
```

---

## Adding Images

### Add an Image to a Section
In `index.html`, add this line where you want the image:
```html
<img src="img/your-image.jpg" alt="Description of image">
```

Replace `your-image.jpg` with your actual image filename.

### Make the Image Smaller
If the image is too big, modify it:
```html
<img src="img/your-image.jpg" alt="Description" width="300">
```

Change `300` to the width you want in pixels.

---

## Adding More Content

### Add a New Paragraph
Just copy and paste an existing `<p>` tag:
```html
<p>Your new paragraph text goes here.</p>
```

### Add a New Bullet Point List
```html
<ul>
    <li>First point</li>
    <li>Second point</li>
    <li>Third point</li>
</ul>
```

### Add a New Service Card
Copy this entire block and paste it where you want:
```html
<div class="card">
    <h3>Your Service Name</h3>
    <p>Describe your service here.</p>
</div>
```

---

## Spacing and Sizing

In `styles.css`, you can adjust spacing with these properties:

- `padding` - space **inside** an element
- `margin` - space **around** an element
- `font-size` - how big text is

Example:
```css
.section {
    padding: 40px;     /* More space inside = more breathing room */
    margin-bottom: 30px; /* More space below = bigger gaps between sections */
}
```

Larger numbers = more space.

---

## Testing Your Changes

1. **Save the file** (Ctrl+S or Cmd+S)
2. **Refresh the browser** (F5 or Cmd+R)
3. You should see your changes immediately

If something looks wrong:
- Check that you didn't accidentally delete anything
- Make sure all quotes (`"` and `'`) are properly closed
- Save the file and refresh again

---

## Common Mistakes to Avoid

❌ **Don't delete these:**
- Opening tags like `<section>` and closing tags like `</section>`
- Quotes around values: `class="header"`
- The curly braces `{}` in CSS

❌ **Don't change:**
- `class`, `id`, or `href` attributes (unless you know what they do)
- CSS property names like `background-color`, `padding`, `font-size`

✅ **Safe to change:**
- Text content between tags
- Color values
- Numbers for sizes and spacing
- Font names

---

## Getting Help

If you get stuck:
1. Undo your last change (Ctrl+Z)
2. Refresh the browser to see the original state
3. Try one change at a time
4. Take a screenshot of what you want it to look like

---

## Next Steps

Once you're comfortable editing, try:
- Adding more sections
- Experimenting with different colors
- Adding images to your pages
- Changing fonts
- Adjusting spacing to your preference

Have fun creating! 🎉
