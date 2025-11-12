# Feel Good News Template Builder - Work Instructions

## Overview
The Feel Good News (FGN) Template Builder is a web-based tool that helps you create formatted HTML content for weekly "Feel Good News" articles. The tool generates a complete HTML template with articles, employee spotlights, and optional "Thank the Donor" sections that can be directly pasted into your content management system.

### Getting Help
- Click the **"📖 View Instructions"** button in the top-right corner of the tool to view these instructions at any time
- The instructions are displayed in a scrollable modal for easy reference while working

---

## Important Prerequisites

### ⚠️ CRITICAL: Publication Date Must Be Set First
**You MUST set the publication date before adding any articles or filling out any content.** The tool will prevent you from adding articles until a date is selected. This date is used to:
- Generate the correct image file paths
- Set schema.org metadata for SEO
- Organize files in the correct date-based folder structure

---

## Order of Operations

### Step 1: Set Publication Date
1. Locate the **"Publication Date"** field at the top of the form
2. Click the date picker and select the publication date for this week's content
3. The warning message will disappear once a date is set
4. **Do not proceed until this step is complete**

### Step 2: Add Articles (Main Stories)
1. Click the **"+ Add Article"** button
2. Fill in the following fields for each article:
   - **Title**: The headline for the article (this will appear in the article header)
   - **Body**: Use the rich text editor to write your article content
     - Formatting options: Bold, Italic, Lists, Links, etc.
     - You can paste formatted text from other sources
   - **Images**: 
     - **For a single image**: Add one image filename (e.g., `photo.jpg`)
     - **For a gallery/slideshow**: Add multiple images (2 or more)
     - **Upload Files**: Click "📁 Upload Files" to bulk upload image files
       - The system will automatically extract filenames and construct full URLs
       - Files are hosted at: `https://www.bloodcenter.org/webres/Image/FGN/MMDDYYYY/`
     - **Image Descriptions/Captions**: Click the **"+"** button next to any image field to add an optional caption/description
       - The caption will appear underneath the image in the output
       - **Important**: Captions automatically function as alt text for accessibility
       - If you add captions, the separate "Image Alt Text" field becomes optional
       - For galleries, each image can have its own caption that displays as you navigate
   - **Image Alt Text**: Required when images are present (unless captions are provided)
     - Describe the image as if describing it to someone who cannot see it
     - Tooltip available for guidance
     - **Note**: If you add captions to your images, those will automatically be used as alt text, making this field optional
   - **Video URL** (optional): Paste a YouTube or Vimeo URL
     - The system will automatically convert it to an embed format
3. Click the arrow (▼) in the article header to collapse/expand articles
4. Use the drag handle (⋮⋮) to reorder articles
5. Click "Remove" to delete an article

### Step 3: Add "Thank the Donor" Section (Optional)
1. Click **"+ Add Thank the Donor"** button (only if you have a thank the donor story this week)
2. Fill in:
   - **Title**: The headline for the thank the donor section
   - **Body**: Content using the rich text editor
   - **Image URL**: Enter just the filename (e.g., `donor-photo.jpg`)
   - **Image Alt Text**: Required when an image is present
3. Click "Remove Section" to delete if needed
4. **Note**: If both "Thank the Donor" and "Employee Spotlight" are present, they will display side-by-side

### Step 4: Fill Out Employee Spotlight
1. Click the **"Employee Spotlight"** header to expand the section (if collapsed)
2. Fill in:
   - **Name**: Employee's full name (default: "First Last")
   - **Job Title**: Employee's position (default: "Job Title")
   - **Image URL**: Enter just the filename (default: `placeholder.jpg`)
3. Answer the default questions:
   - **Time at ImpactLife**: How long the employee has been with the company
   - **Blood Type**: Default is "O Positive" (can be edited)
   - **What runs through your veins?**: Personal interests/passions
   - **What's your favorite thing about being part of our team?**: Team-related answer
   - **When you are not at work you can be found?**: Hobbies/activities outside work
4. **Add/Remove Questions**:
   - Click **"+ Add Question"** to add custom questions
   - Click **"Remove"** on any question/answer pair to delete it
   - You can remove default questions if not needed

### Step 5: Review Preview
1. Check the preview pane on the right side of the screen
2. The preview updates automatically as you type (with a 300ms delay)
3. Verify:
   - All images display correctly
   - Text formatting looks good
   - Article order is correct
   - Employee Spotlight displays properly
   - "Thank the Donor" section appears (if added)

<!-- Step 6: Generate Shareable Content (Optional) - Commented out
### Step 6: Generate Shareable Content (Optional)
1. Click the **"🎨 Shareable Content Studio"** button to create graphics from your content
2. Use the **Quote Cards** tab to extract and download quote graphics
3. Use the **Impact Graphics** tab to create stat cards
4. Download images for use on social media, newsletters, or marketing materials
-->

### Step 6: Copy Generated Code
1. Click the **"Copy Code"** button
2. The complete HTML code is copied to your clipboard
3. Paste it directly into your content management system
4. **Note**: The code includes all necessary CSS, JavaScript, and HTML structure

---

## Image Handling

#### Image File Paths
- **You only need to enter the filename** (e.g., `photo.jpg`)
- The system automatically constructs the full URL using:
  - Base URL: `https://www.bloodcenter.org/webres/Image/FGN/`
  - Date folder: `MMDDYYYY/` (from publication date)
  - Filename: Your entered filename
- **Example**: If date is `2025-10-24` and you enter `photo.jpg`, the full URL becomes:
  `https://www.bloodcenter.org/webres/Image/FGN/10242025/photo.jpg`

#### Single Image vs. Gallery
- **1 image** = Displays as a single static photo (no slideshow)
- **2+ images** = Displays as an interactive gallery/slideshow with navigation controls
- The system automatically detects which format to use based on the number of images

#### Gallery Navigation Features
- **Left/Right Arrows**: Click the arrow buttons to manually navigate through gallery images
- **Auto-Play**: Images automatically advance every 5 seconds
- **Hover to Pause**: Hover your mouse over a gallery image to pause the automatic slideshow
- **Manual Navigation**: Clicking arrows restarts the auto-play timer
- Arrows become more visible when hovering over the gallery

#### Image Captions/Descriptions
- Click the **"+"** button next to any image field to add a caption
- The button changes to **"−"** when the caption field is active
- **Captions serve dual purpose**:
  - Display as visible text underneath the image
  - Automatically function as alt text for accessibility
- **For single images**: Caption displays statically below the image
- **For galleries**: Each image can have its own caption that updates as you navigate
- If you add captions, the separate "Image Alt Text" field becomes optional
- Click **"−"** to hide the caption field (caption text will be cleared)

#### Bulk File Upload
1. Click **"📁 Upload Files"** in the Images section of any article
2. Select multiple image files from your computer
3. The system will:
   - Extract all filenames
   - Construct full URLs automatically
   - Add them to the gallery list
4. You can then edit individual filenames or add captions as needed

### Rich Text Editor
- **Bold** (B), *Italic* (I), Underline (U)
- Bullet lists and numbered lists
- Links (chain icon)
- Text alignment options
- **Pasting Content**: You can paste formatted content from Word, Google Docs, etc.
  - The tool automatically strips inline styles and CSS when pasting
  - This ensures your content uses the template's styling, not external styles
  - Only semantic formatting (bold, italic, lists, links) is preserved

### Video Embeds
- Paste a standard YouTube or Vimeo URL
- Examples:
  - `https://www.youtube.com/watch?v=VIDEO_ID`
  - `https://vimeo.com/VIDEO_ID`
- The system converts it to an embed format automatically

### Reordering Articles
- Click and hold the drag handle (⋮⋮) in the article header
- Drag the article up or down to reorder
- The preview updates automatically
- The order in the form matches the order in the final output

### Collapsible Sections
- Click the arrow (▼/►) in any section header to collapse/expand
- Useful for:
  - Focusing on one article at a time
  - Reducing visual clutter
  - Navigating long forms

---

## Import HTML Feature

### When to Use
- You've already generated HTML and need to make edits
- You want to update an existing Feel Good News page
- You need to add/remove images or modify content

### How to Use
1. Click **"Import HTML"** button
2. Paste the complete HTML code from a previously generated output
3. Click **"Import"**
4. The system will:
   - Extract all article content
   - Extract Employee Spotlight information
   - Extract "Thank the Donor" section (if present)
   - Extract publication date
   - Re-populate all form fields
5. Make your edits
6. Click **"Copy Code"** to generate updated HTML

### Import Limitations
- The import feature works best with HTML generated by this tool
- Complex custom HTML may not import perfectly
- Always review the preview after importing

---

<!-- Shareable Studio Section - Commented out
## Shareable Studio

### Overview
The Shareable Content Studio helps you create engaging graphics and quote cards from your content for use on social media, newsletters, and marketing materials.

### How to Access
1. Click the **"🎨 Shareable Content Studio"** button in the form actions area
2. A modal will open with two tabs: Quote Cards and Impact Graphics

### Quote Cards Tab
1. Click **"🔍 Extract Quotes from Content"** to automatically find compelling quotes from:
   - Article content
   - Employee Spotlight answers
   - Thank the Donor section
2. The system will display up to 12 quote cards with:
   - Beautiful, branded designs using ImpactLife colors
   - Random styling variations for visual interest
   - Quote text and source attribution
3. **Download Options**:
   - Click **"📥 Download Image"** to save a quote card as a PNG file
   - Click **"📋 Copy Text"** to copy just the quote text to your clipboard
4. Use these cards for:
   - Social media posts
   - Newsletter highlights
   - Marketing materials
   - Email campaigns

### Impact Graphics Tab
1. Click **"📊 Generate Impact Graphics"** to create stat cards showing:
   - **Lives Impacted**: Estimated impact based on article count
   - **Stories Shared**: Number of articles
   - **Moments Captured**: Total number of images
   - **Community Impact**: Dedication badge
2. Each graphic features:
   - ImpactLife brand colors
   - Large, readable numbers
   - Professional gradient backgrounds
3. Click **"📥 Download Image"** on any graphic to save it as a PNG file
4. Use these graphics for:
   - Social media posts
   - Impact reports
   - Newsletter headers
   - Presentation slides

### Tips
- Generate quote cards after completing your articles for best results
- The system looks for emotional language, questions, and compelling statements
- Download multiple variations to have options for different platforms
- Impact graphics automatically calculate based on your current content
-->

---

## Tips

### Image Alt Text & Captions
- **Always provide alt text or captions** for images (required by the system)
- **Two ways to provide alt text**:
  1. **Use Image Captions** (Recommended): Click the "+" button next to an image field and add a caption
     - Captions automatically function as both visible text AND alt text
     - One entry serves both purposes - more efficient!
  2. **Use Image Alt Text Field**: Fill in the separate "Image Alt Text" field
     - Required if you don't add captions
     - Optional if you've added captions to your images
- **Best Practice**: Use captions when you want visible text under images, use alt text field when you only need accessibility text
- Describe what's in the image, not just "photo" or "image"
- Think: "If I described this image to someone over the phone, what would I say?"
- Example: "Group of volunteers smiling at a blood drive event" (not just "volunteers")

### Article Titles
- Keep titles concise but descriptive
- The title appears in the article header and updates automatically
- If left blank, defaults to "Article X"

### Employee Spotlight
- All default questions can be edited or removed
- Add custom questions as needed for special features
- The image defaults to a placeholder - remember to update it!

### Preview Pane
- Use the preview to catch formatting issues early
- The preview updates in real-time (300ms delay)
- Scroll position is maintained while typing (no auto-scroll to top)

### File Organization
- Images should be uploaded to: `https://www.bloodcenter.org/webres/Image/FGN/MMDDYYYY/`
- Use the publication date format: `MMDDYYYY` (e.g., `10242025` for October 24, 2025)
- Filenames should be descriptive but not too long

---

## Troubleshooting

### "Please set a publication date" Warning
- **Solution**: Select a date in the "Publication Date" field at the top
- You cannot add articles until a date is set

### Images Not Displaying
- **Check**: Did you enter just the filename (not the full URL)?
- **Check**: Is the publication date set correctly?
- **Check**: Are the image files actually uploaded to the server at the expected path?
- **Check**: Image alt text OR captions are required - make sure at least one is provided
  - You can use the "+" button to add captions (which also function as alt text)
  - Or fill in the "Image Alt Text" field

### Gallery Not Working
- **Check**: Do you have 2 or more images? (1 image = no gallery)
- **Check**: Are all image URLs valid?
- **Check**: Preview the output in a browser to see if JavaScript errors appear
- **Gallery Navigation**:
  - Arrows should appear on the left and right sides of gallery images
  - Hover over the gallery to see arrows more clearly
  - Click arrows to manually navigate
  - Hover over the gallery to pause auto-play

### Can't Add Articles
- **Check**: Is the publication date set?
- **Check**: Are there any JavaScript errors in the browser console?
- **Solution**: Refresh the page and try again

### Import Not Working
- **Check**: Did you paste the complete HTML (including `<html>`, `<head>`, `<body>` tags)?
- **Check**: Is the HTML from a previous version of this tool?
- **Solution**: Try copying the HTML again, ensuring you get the complete code

### Page Scrolling to Top While Typing
- This should be fixed, but if it happens:
- **Solution**: The system should maintain scroll position automatically
- If issues persist, try refreshing the page

### Article Order Not Updating
- **Check**: Did you drag the article using the handle (⋮⋮)?
- **Check**: The preview should update automatically
- **Solution**: Try dragging again or refresh the page

---

## Checklist

Before publishing, verify:
- [ ] Publication date is set
- [ ] All article titles are filled in
- [ ] All article bodies have content
- [ ] All images have alt text OR captions (at least one is required)
- [ ] Image captions are added if you want visible descriptions under images
- [ ] Employee Spotlight name and title are updated (not defaults)
- [ ] Employee Spotlight image is updated (not placeholder)
- [ ] All Employee Spotlight questions are answered
- [ ] Preview looks correct
- [ ] Gallery navigation works (if using galleries)
- [ ] Code has been copied
- [ ] Code has been pasted into CMS and tested

---

## Support Notes

- The tool generates complete, self-contained HTML
- All CSS and JavaScript are included in the output
- The output is ready to paste directly into your CMS
- The preview pane shows exactly how the content will appear
- Real-time updates mean you can see changes immediately

---

## Version Information

- Tool Version: Current as of latest update
- Browser Compatibility: Modern browsers (Chrome, Firefox, Safari, Edge)
- No additional software or plugins required

---

**Last Updated**: Based on current tool functionality
**For Questions or Issues**: Contact your development team

