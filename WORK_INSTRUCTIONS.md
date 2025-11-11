# Feel Good News Template Builder - Work Instructions

## Overview
The Feel Good News (FGN) Template Builder is a web-based tool that helps you create formatted HTML content for weekly "Feel Good News" articles. The tool generates a complete HTML template with articles, employee spotlights, and optional "Thank the Donor" sections that can be directly pasted into your content management system.

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
   - **Image Alt Text**: Required when images are present
     - Describe the image as if describing it to someone who cannot see it
     - Tooltip available for guidance
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

### Step 6: Copy Generated Code
1. Click the **"Copy Code"** button
2. The complete HTML code is copied to your clipboard
3. Paste it directly into your content management system
4. **Note**: The code includes all necessary CSS, JavaScript, and HTML structure

---

## Detailed Feature Explanations

### Image Handling

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
- **2+ images** = Displays as an interactive gallery/slideshow
- The system automatically detects which format to use based on the number of images

#### Bulk File Upload
1. Click **"📁 Upload Files"** in the Images section of any article
2. Select multiple image files from your computer
3. The system will:
   - Extract all filenames
   - Construct full URLs automatically
   - Add them to the gallery list
4. You can then edit individual filenames or add alt text as needed

### Rich Text Editor
- **Bold** (B), *Italic* (I), Underline (U)
- Bullet lists and numbered lists
- Links (chain icon)
- Text alignment options
- You can paste formatted content from Word, Google Docs, etc.

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

## Tips and Best Practices

### Image Alt Text
- **Always provide alt text** for images (required by the system)
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
- **Check**: Image alt text is required - make sure it's filled in

### Gallery Not Working
- **Check**: Do you have 2 or more images? (1 image = no gallery)
- **Check**: Are all image URLs valid?
- **Check**: Preview the output in a browser to see if JavaScript errors appear

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

## Quick Reference Checklist

Before publishing, verify:
- [ ] Publication date is set
- [ ] All article titles are filled in
- [ ] All article bodies have content
- [ ] All images have alt text
- [ ] Employee Spotlight name and title are updated (not defaults)
- [ ] Employee Spotlight image is updated (not placeholder)
- [ ] All Employee Spotlight questions are answered
- [ ] Preview looks correct
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

