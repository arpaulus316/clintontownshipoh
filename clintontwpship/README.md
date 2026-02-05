# Clinton Township Website

Complete website package for Clinton Township, Shelby County, Ohio.

## What's Included

- **index.html** - Main website file (single-page application)
- **forms/** - Folder containing forms
  - application_for_zoning_permit.pdf
  - application_for_zoning_permit.html (standalone)
  - Variance application Page 1.pdf
  - Variance application Page 2.pdf
  - Sign permit.pdf
- **Maps/** - Folder containing maps
  - 2025-08-04_ClintonTwp Zoning MAP.pdf
- **README.md** - This documentation file
- **SETUP_GUIDE.md** - Complete instructions for hosting the website

## Quick Start

1. Upload all files to your web server
2. Ensure the folder structure is maintained (forms folder with files)
3. The website will be immediately accessible

## Features

### Core Pages
- Home page with quick links and township statistics
- Township Trustees & Officials directory
- Zoning Information with board members
- Permits & Forms with downloadable applications
- Interactive Permit Process flowchart (7 steps)
- Events calendar

### Online Zoning Permit Application
- **Fill out online** - Complete the form directly on the website
- **Document uploads** - Attach site plans, building plans, and additional documents
- **Submit online** - Receive confirmation with reference number
- **Print option** - Print the form to mail in instead
- Form validation ensures required fields are completed

### Online Variance Application
- **Fill out online** - Complete variance request on the website
- **Justification sections** - Guided prompts for all 4 required variance criteria
- **Document uploads** - Attach required site plans and supporting documents
- **Submit online** - Receive confirmation with reference number
- **Print option** - Print the form to mail with $200 fee
- **Office Use section** - Includes Board of Zoning Appeals decision area

### Online Sign Permit Application (NEW)
- **Fill out online** - Complete sign permit request on the website
- **Sign details** - Type, size, height, electric, replacing existing
- **Auto-calculate** - Sign area calculated automatically from dimensions
- **Document uploads** - Attach plot plan and sign design
- **Submit online** - Receive confirmation with reference number
- **Print option** - Print the form to mail with $25 fee
- **Office Use section** - Approval tracking

### Design Features
- Mobile responsive design
- Professional government styling
- Single-page application (fast navigation)
- Print-optimized form styling for each form

## File Structure

```
clintontwpship/
├── index.html                              # Main website
├── README.md                               # This file
├── SETUP_GUIDE.md                          # Hosting instructions
├── forms/
│   ├── application_for_zoning_permit.pdf   # Zoning permit PDF
│   ├── application_for_zoning_permit.html  # Standalone HTML form
│   ├── Variance application Page 1.pdf     # Variance PDF
│   ├── Variance application Page 2.pdf     # Variance PDF (office use)
│   └── Sign permit.pdf                     # Sign permit PDF
├── Maps/
│   └── 2025-08-04_ClintonTwp Zoning MAP.pdf  # Township zoning map
└── files/
    └── (original files)
```

## Website Pages

| Page | Description |
|------|-------------|
| Home | Welcome page with quick links, stats, and service cards |
| Officials | Trustees and township staff contact information |
| Zoning | Zoning department info and commission members |
| Permits | Downloadable forms and fee schedule |
| Permit Process | Step-by-step flowchart for obtaining permits |
| Zoning Permit Form | Online zoning permit application |
| Variance Form | Online variance application |
| **Sign Permit Form** | **Online sign permit application** |
| Events | Upcoming township meetings and events |

## Running Locally

To test the website on your local computer:

```bash
# Using Python
python -m http.server 8000

# Then open: http://localhost:8000
```

## Technical Details

- **Framework:** Pure HTML/CSS/JavaScript (no dependencies)
- **Browser Support:** All modern browsers (Chrome, Firefox, Edge, Safari)
- **Mobile:** Fully responsive design
- **Hosting:** Works with any web host
- **Form Submission:** Client-side only (requires backend for actual submission)

## Contact Information

Currently configured with:
- **Board of Trustees:** Dave Wood (Chairman), Todd Ratterman, Jim Gaier
- **Fiscal Officer:** Sally Wood, 937-726-0357, swood081959@hotmail.com
- **Zoning Officer:** Rick Paulus, 937-538-9895, rickjp79@outlook.com, 680 Doorley Rd, Sidney, Ohio
- **Zoning Commission:** Bonnie Deck (Chair), Greg Mericle (V. Chair), Jeff Iwanski, Gary Mericle
- **Board of Zoning Appeals:** Amy Berger (Chair), Don Douglas (V. Chair), Jeff Wheeler, Tony J. Strunk, Vacant

## Permit Fee Information (2026)

| Permit Type | Fee |
|-------------|-----|
| Building Permit | $2.00 per $1,000 (min $150, max $500) |
| Sign Permit | $75 + $0.50/sq ft (max $150) |
| Zoning Code Change | $550.00 |
| Zoning Map Change | $550.00 |
| Zoning Board Hearings | $375.00 |
| **Sign Permit** | **$25.00** |
| Zoning Map Amendment | $300.00 |
| Conditional Use Permit | $150.00 |

Construction fee: $2 per $1,000 of construction cost ($100 min, $400 max)

## Sign Permit Requirements

- **Sign Types:** Attached, Detached, Interstate, Advertising (off site)
- **Required Info:** Sign dimensions, height from ground, electric (yes/no)
- **Required Documents:**
  - Plot plan showing sign placement relative to property lines and buildings
  - Proposed sign dimensions including height from ground
  - Sign design/rendering (optional)

## Customization Notes

### To Add Real Form Submission
The online forms currently show a confirmation modal. To actually receive submissions:
1. Use a form service like Formspree, Netlify Forms, or Google Forms
2. Or set up a backend server to receive the form data
3. Update the form's `action` attribute and method

### To Update Events
Edit the events section in `index.html` to add real township events.

### To Add More Forms
1. Add PDF files to the `forms/` folder
2. Update the downloads-grid section in `index.html`
3. Optionally create an online form page following the existing patterns

---

**Created:** January 2026
**Version:** 2.2 (with online zoning permit, variance, and sign permit applications)
