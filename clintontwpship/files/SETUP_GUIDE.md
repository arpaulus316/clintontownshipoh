# Clinton Township Website - Setup Guide

## File Structure

To make the website work with the PDF forms, you'll need to organize your files as follows:

```
your-website/
├── index.html (rename clinton-township.html to this)
├── forms/
│   ├── application_for_zoning_permit.pdf
│   ├── variance_application.pdf (to be added)
│   ├── sign_permit_application.pdf (to be added)
│   └── fee_schedule.pdf (to be added)
└── maps/
    └── zoning_map.pdf (to be added)
```

## Step-by-Step Setup Instructions

### Step 1: Prepare Your Files

1. **Rename the HTML file:**
   - Rename `clinton-township.html` to `index.html`

2. **Create folders:**
   - Create a folder called `forms`
   - Create a folder called `maps`

3. **Place your PDF files:**
   - Put `application_for_zoning_permit.pdf` in the `forms` folder
   - Add other form PDFs as you create them

### Step 2: Upload to Your Web Server

You have several options for hosting:

#### Option A: Traditional Web Hosting
1. Use an FTP client (like FileZilla) to connect to your web host
2. Upload the `index.html` file to your public_html or www directory
3. Upload the `forms` and `maps` folders with all PDFs

#### Option B: Free Hosting Options
- **GitHub Pages** (free, recommended for small sites)
  1. Create a GitHub account
  2. Create a new repository named `clinton-township`
  3. Upload all files
  4. Enable GitHub Pages in repository settings
  
- **Netlify** (free tier available)
  1. Create account at netlify.com
  2. Drag and drop your folder
  3. Get instant deployment

#### Option C: Township Web Server
- Work with your township's IT department or web administrator
- Provide them with all the files
- They can integrate it into your existing township website

### Step 3: Test the Website

After uploading, test these features:
1. Click on "Permits & Forms" - verify PDF downloads work
2. Click on "Permit Process" - check the flowchart displays correctly
3. Test all navigation links
4. Verify on mobile devices

### Step 4: Update Contact Information

Before going live, update these placeholders:
1. **Regulations Link** (Regulations page):
   - Replace `#` with actual URL to your regulations portal

2. **Events** (Events page):
   - Update with real township events and dates

### Step 5: Add Missing Forms

As you create or scan additional forms, add them to the website:

1. **Variance Application** - Add PDF to `forms/` folder
2. **Sign Permit Application** - Add PDF to `forms/` folder  
3. **Fee Schedule** - Add PDF to `forms/` folder
4. **Zoning Map** - Add PDF to `maps/` folder

The website is already configured to link to these files at:
- `forms/variance_application.pdf`
- `forms/sign_permit_application.pdf`
- `forms/fee_schedule.pdf`
- `maps/zoning_map.pdf`

## PDF File Requirements

- **File Format:** PDF (preferred) or fillable PDF forms
- **File Size:** Keep under 5MB for faster downloads
- **Naming:** Use lowercase, underscores instead of spaces
- **Examples:** 
  - ✓ `application_for_zoning_permit.pdf`
  - ✗ `Application for Zoning Permit.pdf`

## Making Forms Fillable (Optional)

You can create fillable PDF forms using:
- Adobe Acrobat Pro
- PDFescape (free online tool)
- LibreOffice (free)

This allows residents to fill out forms on their computer before printing.

## Security Considerations

1. **Forms Only:** Only upload blank forms, never completed applications
2. **No Personal Data:** Never put residents' personal information on the website
3. **HTTPS:** Ensure your hosting uses HTTPS (secure connection)

## Maintenance

### Regular Updates Needed:
- **Events Page:** Update monthly with new events
- **Trustee Information:** Update when officials change
- **Contact Information:** Keep phone numbers and addresses current
- **Forms:** Update when zoning regulations change

### Optional Enhancements:
- Add a contact form using a service like Formspree or Google Forms
- Integrate Google Calendar for events
- Add a news/announcements section
- Include photo gallery of township

## Support Resources

If you need help with:
- **Web Hosting:** Contact your township's IT department
- **Domain Names:** Register at services like GoDaddy or Namecheap
- **Technical Issues:** Most web hosts offer support

## Current Website Features

✓ Home page with quick links
✓ Township Trustees & Officials page
✓ Zoning Information page
✓ Permits & Forms page
✓ Permit Process flowchart
✓ Events page
✓ Regulations page (link to external site)
✓ Mobile responsive design
✓ Professional styling
✓ Easy navigation

## Questions?

For questions about the website content or technical setup, contact:
- **Zoning Officer:** Jim Bowser, 638-2587
- **Fiscal Officer:** Tyler J. Morris, 710-1435

---

**Note:** The website has been configured with the correct file paths. Once you upload the PDF files to the `forms` folder, the download links will work automatically.