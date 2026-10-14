# How to Update Your Website

## Adding a New Blog Post (Paper Summary)

1. **Create a new file** in the `_posts` folder with this naming format:
   ```
   YYYY-MM-DD-title-of-post.md
   ```
   Example: `2026-10-15-wealth-of-nations.md`

2. **Copy the template** from `_posts/TEMPLATE.md` or use this structure:
   ```markdown
   ---
   layout: post
   title: "Your Paper Title"
   date: 2026-10-15
   ---

   Your summary text here...
   ```

3. **Write your summary** below the `---` section

4. **Save the file** and commit to GitHub - it will automatically appear on your blog page!

## Customizing Colors and Fonts

Edit `/assets/css/style.css` at the top where it says "Customizable variables":

```css
:root {
    --background-color: #4a0000;  /* Change this for different background */
    --text-color: #ffffff;        /* Change text color */
    --link-color: #ffffff;        /* Change link color */
    --link-hover-color: #cccccc;  /* Change link hover color */
    --font-family: 'Times New Roman', Times, serif;  /* Change font */
    --font-size: 18px;            /* Change base font size */
    --max-width: 700px;           /* Change content width */
}
```

### Example color changes:
- Darker red: `#3a0000`
- Burgundy: `#800020`
- Navy blue: `#001f3f`
- Black: `#000000`

### Example font changes:
- Georgia: `'Georgia', serif`
- Garamond: `'Garamond', serif`
- Modern sans: `'Helvetica', 'Arial', sans-serif`

## Updating the About Page

Edit `/index.md` to change your about-me text on the landing page.

## Publishing Changes

1. **Save your changes** in your editor
2. **Open GitHub Desktop**
3. **Review changes** in the left panel
4. **Write a commit message** (e.g., "Add new paper summary")
5. **Click "Commit to main"**
6. **Click "Push origin"** to publish

Your changes will be live at victoriawyan.com in 1-2 minutes!

## Adding an Image to Landing Page

1. Put your image in `/assets/` folder
2. Edit `/assets/css/style.css` and add to `.home-content`:
   ```css
   .home-content img {
       max-width: 300px;
       border-radius: 4px;
       margin: 20px 0;
   }
   ```
3. Edit `/index.md` and add:
   ```markdown
   ![Your photo](/assets/your-image-name.jpg)
   ```
