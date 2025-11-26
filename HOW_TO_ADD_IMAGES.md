# How to Add Your Own Images to the Portfolio

## Quick Start

### Step 1: Create an Images Folder
1. Create a new folder called `images` in your `reflection-portfolio` folder
2. Put all your photos in this folder

### Step 2: Replace Placeholder Images in HTML

Find these lines in `index.html` and replace the placeholder URLs with your image paths:

#### Part 1 - Relating Lessons to Current Self
```html
<!-- Replace these three images -->
<img src="images/your-photo1.jpg" alt="Reflection moment 1">
<img src="images/your-photo2.jpg" alt="Reflection moment 2">
<img src="images/your-photo3.jpg" alt="Reflection moment 3">
```

#### Part 2 - Summary of Interviews
```html
<!-- Replace these two images -->
<img src="images/interview-photo1.jpg" alt="Interview moment 1">
<img src="images/interview-photo2.jpg" alt="Interview moment 2">
```

#### Part 3 - Manifestos
```html
<!-- Replace this wide image -->
<img src="images/manifesto-photo.jpg" alt="Visual representation of your manifesto">
```

### Step 3: Update Captions
Update the text inside `<p class="image-caption">` tags to describe each image.

## Example

**Current (Placeholder):**
```html
<div class="gallery-item">
    <img src="https://via.placeholder.com/800x600/a67c7c/ffffff?text=Your+Image+1" alt="Reflection moment 1">
    <p class="image-caption">Add your image caption here - describe this moment</p>
</div>
```

**After (Your Image):**
```html
<div class="gallery-item">
    <img src="images/my-reflection.jpg" alt="Reflection moment 1">
    <p class="image-caption">This photo shows my journey through self-discovery during my first year of college.</p>
</div>
```

## Supported Image Formats
- `.jpg` or `.jpeg`
- `.png`
- `.gif`
- `.webp`

## Tips
1. **Image size**: Try to keep images under 2MB for faster loading
2. **Resolution**: 800x600 pixels or higher recommended
3. **Naming**: Use descriptive names like `interview-with-mom.jpg` instead of `IMG_1234.jpg`
4. **Alt text**: Always update the `alt=""` attribute to describe what's in the image

## Adding More Images

To add more images to any section, copy this block:

```html
<div class="gallery-item">
    <img src="images/your-new-photo.jpg" alt="Description">
    <p class="image-caption">Your caption here</p>
</div>
```

Paste it inside the `<div class="image-gallery">` section where you want it to appear.

## Removing Images

To remove an image, simply delete the entire `<div class="gallery-item">...</div>` block.

## Full Example Section

```html
<div class="image-gallery">
    <div class="gallery-item">
        <img src="images/reflection1.jpg" alt="My first reflection">
        <p class="image-caption">Starting my journey of self-discovery</p>
    </div>
    <div class="gallery-item">
        <img src="images/reflection2.jpg" alt="Growing stronger">
        <p class="image-caption">Overcoming challenges and growing stronger</p>
    </div>
    <div class="gallery-item">
        <img src="images/reflection3.jpg" alt="Current state">
        <p class="image-caption">Where I am today and where I'm heading</p>
    </div>
</div>
```

## Need Help?
If images aren't showing:
1. Check that the image file is in the `images` folder
2. Make sure the filename matches exactly (case-sensitive!)
3. Check that you're using forward slashes: `images/photo.jpg` not `images\photo.jpg`
