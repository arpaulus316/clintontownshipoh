# Clinton Township Website - Setup Guide

## File Structure

```
clintontwpship/
├── index.html                              # Main website
├── README.md                               # Documentation
├── SETUP_GUIDE.md                          # This file
├── forms/
│   ├── application_for_zoning_permit.pdf   # Zoning permit PDF
│   ├── application_for_zoning_permit.html  # Standalone HTML form
│   ├── Variance application Page 1.pdf     # Variance PDF
│   ├── Variance application Page 2.pdf     # Variance PDF (office use)
│   └── Sign permit.pdf                     # Sign permit PDF
├── Maps/
│   └── 2025-08-04_ClintonTwp Zoning MAP.pdf  # Township zoning map
└── files/                                  # Original files (optional)
```

## Step-by-Step Setup Instructions

### Step 1: Prepare Your Files

Your website is ready to use. The main files you need are:
- `index.html` - The complete website
- `forms/` folder - Contains all permit forms

### Step 2: Upload to Your Web Server

#### Option A: Traditional Web Hosting
1. Use an FTP client (like FileZilla) to connect to your web host
2. Upload `index.html` to your public_html or www directory
3. Upload the `forms` folder with all files inside

#### Option B: Free Hosting Options

**GitHub Pages** (free, recommended)
1. Create a GitHub account at github.com
2. Create a new repository named `clinton-township`
3. Upload all files maintaining the folder structure
4. Go to Settings > Pages > Enable GitHub Pages
5. Your site will be live at `https://yourusername.github.io/clinton-township`

**Netlify** (free tier available)
1. Create account at netlify.com
2. Drag and drop your entire folder
3. Get instant deployment with HTTPS

### Step 3: Test the Website

After uploading, verify these features work:

1. **Navigation** - Click all menu items
2. **Zoning Permit Form** - Opens from "Apply for Permit" button
3. **Variance Form** - Available from Permits page
4. **Sign Permit Form** - Available from Permits page
5. **Form Submission** - Fill out and submit (shows confirmation)
6. **Document Upload** - Test file selection
7. **Print Forms** - Click print button, verify print preview
8. **PDF Downloads** - Download PDFs from Permits page
9. **Mobile** - Test on phone/tablet

### Step 4: Configure Form Submission (Optional)

The forms currently show a confirmation message but don't actually send data anywhere. To receive submissions:

#### Option 1: Formspree (Easiest)
1. Sign up at formspree.io (free tier: 50 submissions/month)
2. Get your form endpoint URL
3. Update the form tags in index.html:
```html
<form id="zoningPermitForm" action="https://formspree.io/f/YOUR_ID" method="POST">
<form id="varianceForm" action="https://formspree.io/f/YOUR_ID" method="POST">
<form id="signPermitForm" action="https://formspree.io/f/YOUR_ID" method="POST">
```

#### Option 2: Netlify Forms (If using Netlify hosting)
1. Add `netlify` attribute to your forms
2. Submissions appear in your Netlify dashboard

## Website Features Overview

### Online Forms Available

| Form | Fee | Features |
|------|-----|----------|
| Zoning Permit | $50-$100 | Property info, construction details, document upload |
| Variance Application | $200 | Justification sections (a-d), Board of Appeals decision |
| Sign Permit | $25 | Sign type/size, auto-calculate area, placement plan |

### Print Functionality
When users click "Print & Mail Instead":
- Navigation and buttons are hidden
- Only the form content prints
- Upload section is hidden
- Mailing address is shown
- Each form prints correctly when its print button is clicked

## Troubleshooting

### Forms Not Downloading
- Verify the `forms` folder is uploaded
- Check file names match exactly (case-sensitive)
- Ensure files have proper permissions

### Page Not Loading
- Verify `index.html` is in the root directory
- Check for JavaScript errors in browser console (F12)
- Clear browser cache

### Print Not Working
- Try a different browser
- Check if pop-up blocker is interfering
- Use Ctrl+P as alternative

## Fee Schedule (2026)

| Permit Type | Fee |
|-------------|-----|
| Building Permit | $2.00 per $1,000 (min $150, max $500) |
| Sign Permit | $75 + $0.50/sq ft (max $150) |
| Zoning Code Change | $550.00 |
| Zoning Map Change | $550.00 |
| Zoning Board Hearings | $375.00 |

## Contact Information

**Configured Officials:**
- Board of Trustees: Dave Wood (Chairman), Todd Ratermann, Jim Gaier
- Fiscal Officer: Sally Wood, 937-726-0357, swood081959@hotmail.com
- Zoning Officer: Rick Paulus, 937-538-9895, rickjp79@outlook.com, 680 Doorley Rd, Sidney, Ohio
- Zoning Commission: Bonnie Deck (Chair), Greg Mericle (V. Chair), Jeff Iwanski, Gary Mericle
- Board of Zoning Appeals: Amy Berger (Chair), Don Douglas (V. Chair), Jeff Wheeler, Tony J. Strunk, Vacant

**To update contact info:**
Search for the name in `index.html` and update all occurrences.

## Technical Specifications

| Specification | Value |
|---------------|-------|
| HTML Version | HTML5 |
| CSS | Embedded (no external files) |
| JavaScript | Vanilla JS (no frameworks) |
| Dependencies | None (Google Fonts optional) |
| File Size | ~100KB (index.html) |
| Browser Support | Chrome, Firefox, Edge, Safari |

---

**Last Updated:** January 2026
**Version:** 2.2
