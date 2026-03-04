# Acting Portfolio Guide

This guide will help you add acting portfolio items to your website.

## How to Add Acting Portfolio Items

1. **Locate the Acting Section** in `index.html` (around line 450)

2. **Replace the placeholder** with the acting grid structure:

```html
<!-- Remove this placeholder section: -->
<div class="acting-placeholder">
    <p>Acting portfolio items coming soon! This section will showcase performances, headshots, and experience.</p>
</div>

<!-- Replace with this: -->
<div class="acting-grid">
    <!-- Add your acting items here -->
</div>
```

3. **Add Acting Items** using this template:

```html
<div class="acting-item">
    <div class="acting-image">
        <!-- Option 1: Add an image -->
        <img src="images/your-photo.jpg" alt="Production name" style="width: 100%; height: 100%; object-fit: cover;">
        
        <!-- Option 2: Keep placeholder text if no image yet -->
        <!-- Photo coming soon -->
    </div>
    <div class="acting-info">
        <h3>Production Name</h3>
        <div class="role">Role: Character Name</div>
        <div class="details">Theater/Company • Year</div>
    </div>
</div>
```

## Example with Multiple Productions

```html
<div class="acting-grid">
    <div class="acting-item">
        <div class="acting-image">
            <img src="images/hamlet.jpg" alt="Hamlet" style="width: 100%; height: 100%; object-fit: cover;">
        </div>
        <div class="acting-info">
            <h3>Hamlet</h3>
            <div class="role">Role: Ophelia</div>
            <div class="details">University Theater • 2025</div>
        </div>
    </div>

    <div class="acting-item">
        <div class="acting-image">
            <img src="images/musical.jpg" alt="The Music Man" style="width: 100%; height: 100%; object-fit: cover;">
        </div>
        <div class="acting-info">
            <h3>The Music Man</h3>
            <div class="role">Role: Marian Paroo</div>
            <div class="details">Community Theater • 2024</div>
        </div>
    </div>

    <div class="acting-item">
        <div class="acting-image">
            Photo coming soon
        </div>
        <div class="acting-info">
            <h3>A Midsummer Night's Dream</h3>
            <div class="role">Role: Puck</div>
            <div class="details">High School Production • 2021</div>
        </div>
    </div>
</div>
```

## Adding Images

1. Create an `images` folder in your repository:
   ```bash
   mkdir images
   ```

2. Add your photos to the `images` folder

3. Reference them in the HTML:
   ```html
   <img src="images/your-photo.jpg" alt="Description">
   ```

4. Commit and push to GitHub:
   ```bash
   git add images/
   git add index.html
   git commit -m "Add acting portfolio images"
   git push
   ```

## Tips

- **Image Size**: For best results, use images that are at least 600x400 pixels
- **File Format**: JPG or PNG work best
- **File Names**: Use lowercase with hyphens (e.g., `hamlet-2025.jpg`)
- **Alt Text**: Always include descriptive alt text for accessibility
- **Order**: List productions in reverse chronological order (newest first)

## Adding More Details

You can expand the details section to include more information:

```html
<div class="details">
    Theater/Company • Year<br>
    Director: Name<br>
    Additional notes or awards
</div>
```

## Need Help?

If you need to make changes to the styling or layout, the CSS for the acting section starts around line 240 in `index.html`.
