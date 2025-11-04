# John's Handyman Landing Page - Maintenance & Customization Guide

Welcome! This comprehensive guide will help you maintain and customize your John's Handyman landing page. Whether you're updating text, fixing links, or adding new pages, you'll find clear, step-by-step instructions below.

---

## Table of Contents

1. [Understanding the Page Structure](#understanding-the-page-structure)
2. [Updating Text Content](#updating-text-content)
3. [Modifying Tailwind CSS Classes](#modifying-tailwind-css-classes)
4. [Fixing and Managing Links](#fixing-and-managing-links)
5. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
6. [Common Customization Tasks](#common-customization-tasks)
7. [Troubleshooting Guide](#troubleshooting-guide)

---

## Understanding the Page Structure

### Page Sections Overview

Your landing page is organized into distinct sections, each serving a specific purpose:

| Section | ID/Location | Purpose |
|---------|------------|---------|
| Header & Navigation | `<header>` | Main menu and branding |
| Hero Section | First `<section>` | Eye-catching introduction |
| Features Section | `id="features"` | Why Choose Us section |
| Benefits Section | `id="benefits"` | How We Transform Your Life |
| About Section | `id="about"` | Company background |
| Testimonials | `id="testimonials"` | Customer reviews |
| FAQ Section | `id="faq"` | Frequently Asked Questions |
| CTA Section | Before `<footer>` | Call-to-Action |
| Footer | `<footer>` | Contact info & links |

### Key Files You'll Work With

- **index.html** - Main landing page (the file provided)
- **privacy.html** - Privacy Policy page (needs to be created or linked)
- **terms.html** - Terms of Service page (needs to be created or linked)
- **blog.html** - Blog page (optional, referenced in footer)

---

## Updating Text Content

### How to Edit Text - The Basics

Text on your website lives between opening and closing HTML tags. Here's what to look for:

```html
<h1>This is a heading</h1>
<p>This is a paragraph of text</p>
<span>This is inline text</span>
```

**To change any text:**
1. Open `index.html` in a text editor (like Notepad, VS Code, or Sublime Text)
2. Find the text you want to change
3. Replace it with your new text
4. Save the file (Ctrl+S or Cmd+S)
5. Refresh your browser to see changes

### Specific Text Locations to Update

#### Header/Navigation Section

**Location:** Lines 45-60 (approximately)

The header contains your business name and navigation menu:

```html
<div class="flex items-center gap-2">
    <i class="fas fa-tools text-blue-600 text-2xl"></i>
    <h1 class="text-2xl font-bold text-gray-900">John's Handyman</h1>
</div>
```

**To change the business name:**
- Find `John's Handyman` in the header
- Replace with your business name
- **Important:** Do this in TWO places:
  1. In the header (line ~52)
  2. In the footer (line ~436)

**Example:**
```html
<!-- Change from: -->
<h1 class="text-2xl font-bold text-gray-900">John's Handyman</h1>

<!-- Change to: -->
<h1 class="text-2xl font-bold text-gray-900">Mike's Handyman Services</h1>
```

#### Hero Section (Main Introduction)

**Location:** Lines 75-120 (approximately)

This is the large headline and description at the top of the page:

```html
<h1 class="text-4xl sm:text-5xl lg:text-6xl font-bold text-gray-900 mb-6 leading-tight tracking-tight">
    We Provide Quality <span class="gradient-accent bg-clip-text text-transparent">For Less</span>
</h1>

<p class="text-lg sm:text-xl text-gray-600 mb-8 max-w-2xl mx-auto leading-relaxed">
    Transform your home with professional, affordable handyman services...
</p>
```

**To update the hero headline:**
- Keep the main text but change "For Less" to your value proposition
- **Example:** "We Provide Quality <span class="gradient-accent bg-clip-text text-transparent">At Unbeatable Prices</span>"

**To update the hero description:**
- Replace the entire paragraph with your own description
- Keep it between 2-3 sentences for best results
- Keep the same HTML structure (the `<p>` tag)

#### Feature Cards (Why Choose Our Services)

**Location:** Lines 165-230 (approximately)

Each feature has a title and bullet points:

```html
<h3 class="text-2xl font-bold text-gray-900 mb-4">Affordable Pricing</h3>
<p class="text-gray-700 mb-4">Get premium handyman services without breaking the bank...</p>
<ul class="space-y-2 text-gray-600">
    <li class="flex items-center gap-2">
        <i class="fas fa-check text-green-600"></i>
        <span>Transparent pricing with no hidden fees</span>
    </li>
```

**To update feature titles and descriptions:**
1. Find the `<h3>` tag with the feature title
2. Replace the text
3. Update the paragraph below it
4. Update the bullet points in the `<ul>` list

**Example:**
```html
<!-- Original: -->
<h3 class="text-2xl font-bold text-gray-900 mb-4">Affordable Pricing</h3>

<!-- Updated: -->
<h3 class="text-2xl font-bold text-gray-900 mb-4">Budget-Friendly Solutions</h3>
```

#### Benefits Section (How We Transform Your Life)

**Location:** Lines 260-310 (approximately)

Similar structure to features:

```html
<h3 class="text-2xl font-bold text-gray-900 mb-3">Relax and Unwind</h3>
<p class="text-gray-700 mb-4">Stop stressing about home repairs...</p>
```

**Update process:** Same as Feature Cards above

#### About Section

**Location:** Lines 340-380 (approximately)

Contains your company story:

```html
<h2 class="text-4xl md:text-5xl font-bold text-gray-900 mb-8">About John's Handyman</h2>

<p class="text-lg text-gray-700 mb-6 leading-relaxed">
    John's Handyman was founded over 15 years ago with a simple mission...
</p>
```

**To update the About section:**
1. Change the heading from "About John's Handyman" to "About [Your Business Name]"
2. Replace the company story paragraphs with your own
3. Update the statistics (15+ Years, 2000+ Happy Customers)

**Important locations to update:**
- Line ~354: Company name in heading
- Lines ~357-365: First paragraph (company history)
- Lines ~367-372: Second paragraph (company values)
- Line ~385: Years of experience number
- Line ~397: Customer count number

#### Testimonials Section

**Location:** Lines 415-505 (approximately)

Each testimonial has a quote and customer name:

```html
<p class="text-gray-700 mb-4 leading-relaxed">
    "John fixed our kitchen sink in under an hour and the price was half..."
</p>
<div class="border-t pt-4">
    <p class="font-bold text-gray-900">Sarah Mitchell</p>
    <p class="text-sm text-gray-600">Homeowner, Downtown</p>
</div>
```

**To update testimonials:**
1. Replace the quoted text with real customer feedback
2. Update the customer name
3. Update the customer title/description
4. Keep the 5-star rating (the stars are created with icons)

#### FAQ Section

**Location:** Lines 535-650 (approximately)

Each FAQ item has a question and answer:

```html
<button class="faq-question w-full px-6 py-4 text-left flex items-center justify-between...">
    <span class="text-lg font-semibold text-gray-900">What types of services do you offer?</span>
</button>
<div class="faq-answer hidden px-6 py-4 bg-white border-t border-gray-200">
    <p class="text-gray-700 leading-relaxed">We offer a comprehensive range...</p>
</div>
```

**To update FAQ items:**
1. Find the question in the `<span>` tag
2. Replace with your question
3. Find the answer in the `<p>` tag below
4. Replace with your answer
5. **Do NOT change** the `class` attributes - they control the accordion functionality

#### Footer Section

**Location:** Lines 700-850 (approximately)

Footer contains company info, links, and contact details:

```html
<h3 class="text-xl font-bold text-white">John's Handyman</h3>
<p class="text-gray-400 mb-4">Providing quality handyman services at affordable prices since 2010.</p>
```

**Key footer elements to update:**
- Business name (line ~714)
- Tagline/description (line ~716)
- Email address (line ~810)
- Phone number (line ~814)
- Business hours (line ~818)
- Copyright year (line ~850)

**Example:**
```html
<!-- Original: -->
<p class="text-gray-400 mb-4">Providing quality handyman services at affordable prices since 2010.</p>

<!-- Updated: -->
<p class="text-gray-400 mb-4">Professional home repair and maintenance services since 2008.</p>
```

### Important: Meta Tags (Search Engine Information)

**Location:** Lines 5-10 (in the `<head>` section)

These tags help search engines understand your page:

```html
<meta name="description" content="John's Handyman Site - Quality handyman services at affordable prices...">
<meta name="keywords" content="handyman, home repair, affordable, reliable, quality service">
<meta name="author" content="John's Handyman">
<title>John's Handyman Site - Quality Services for Less</title>
```

**Update these with your information:**
- **description:** 150-160 characters describing your business
- **keywords:** Comma-separated words people search for
- **author:** Your business name
- **title:** Your page title (appears in browser tab)

**Example:**
```html
<meta name="description" content="Mike's Professional Handyman - Expert home repairs at affordable rates. Plumbing, electrical, carpentry & more.">
<meta name="keywords" content="handyman services, home repair, plumbing, electrical, carpentry">
<meta name="author" content="Mike's Professional Handyman">
<title>Mike's Professional Handyman - Expert Home Repairs</title>
```

---

## Modifying Tailwind CSS Classes

### What Are Tailwind CSS Classes?

Tailwind CSS is a system that uses short class names to style your website. Instead of writing custom CSS code, you add class names to HTML elements.

**Example:**
```html
<div class="bg-blue-600 text-white px-8 py-4 rounded-lg">
    This is a blue button with white text
</div>
```

Breaking this down:
- `bg-blue-600` = Blue background color
- `text-white` = White text color
- `px-8` = Padding (space inside) left and right
- `py-4` = Padding (space inside) top and bottom
- `rounded-lg` = Rounded corners

### Common Tailwind Classes in Your Landing Page

#### Colors

```html
<!-- Background Colors -->
<div class="bg-white">White background</div>
<div class="bg-gray-50">Light gray background</div>
<div class="bg-blue-600">Blue background</div>
<div class="bg-green-600">Green background</div>
<div class="bg-purple-600">Purple background</div>

<!-- Text Colors -->
<p class="text-gray-900">Dark gray text</p>
<p class="text-gray-600">Medium gray text</p>
<p class="text-white">White text</p>
<p class="text-blue-600">Blue text</p>
```

**To change a color:**
1. Find the color class you want to change
2. Replace it with a new color class

**Example - Change a button from blue to green:**
```html
<!-- Original: -->
<a href="..." class="bg-blue-600 text-white px-8 py-4 rounded-lg">
    Get Started
</a>

<!-- Updated: -->
<a href="..." class="bg-green-600 text-white px-8 py-4 rounded-lg">
    Get Started
</a>
```

**Available color options:**
- Gray: `gray-50`, `gray-100`, `gray-200`, `gray-600`, `gray-900`
- Blue: `blue-50`, `blue-100`, `blue-600`, `blue-700`
- Green: `green-50`, `green-100`, `green-600`
- Purple: `purple-50`, `purple-600`
- Red: `red-600`, `red-700`
- Yellow: `yellow-400`

#### Spacing (Padding & Margins)

Tailwind uses a scale from 0-96 for spacing:

```html
<!-- Padding (space inside) -->
<div class="p-4">Padding all sides</div>
<div class="px-8">Padding left and right</div>
<div class="py-4">Padding top and bottom</div>
<div class="pt-6">Padding top only</div>

<!-- Margin (space outside) -->
<div class="m-4">Margin all sides</div>
<div class="mb-6">Margin bottom</div>
<div class="mt-8">Margin top</div>
```

**Scale reference:**
- `1` = 4px
- `2` = 8px
- `4` = 16px
- `6` = 24px
- `8` = 32px
- `12` = 48px
- `16` = 64px
- `24` = 96px

**Example - Increase button padding:**
```html
<!-- Original (smaller button): -->
<a class="px-6 py-2 rounded-lg">Get Started</a>

<!-- Updated (larger button): -->
<a class="px-8 py-4 rounded-lg">Get Started</a>
```

#### Text Sizing & Styling

```html
<!-- Font Sizes -->
<h1 class="text-6xl">Very large heading</h1>
<h2 class="text-4xl">Large heading</h2>
<p class="text-lg">Large paragraph</p>
<p class="text-base">Normal paragraph</p>
<p class="text-sm">Small text</p>

<!-- Font Weight -->
<p class="font-bold">Bold text</p>
<p class="font-semibold">Semi-bold text</p>
<p class="font-medium">Medium weight</p>
<p class="font-normal">Normal weight</p>

<!-- Text Alignment -->
<div class="text-center">Centered text</div>
<div class="text-left">Left-aligned text</div>
<div class="text-right">Right-aligned text</div>
```

#### Responsive Design Classes

Your page needs to look good on phones, tablets, and computers. Tailwind uses prefixes for different screen sizes:

```html
<!-- Mobile first, then larger screens -->
<h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl">
    Responsive heading
</h1>
```

Breaking this down:
- `text-2xl` = 24px on mobile phones
- `sm:text-3xl` = 30px on small tablets and up
- `md:text-4xl` = 36px on medium tablets and up
- `lg:text-5xl` = 48px on large screens and up

**Breakpoints:**
- `sm:` = 640px and up (small tablets)
- `md:` = 768px and up (tablets)
- `lg:` = 1024px and up (large tablets and desktops)
- `xl:` = 1280px and up (large desktops)

**Example - Adjust heading sizes:**
```html
<!-- Original: -->
<h1 class="text-4xl sm:text-5xl lg:text-6xl">We Provide Quality</h1>

<!-- Make smaller: -->
<h1 class="text-3xl sm:text-4xl lg:text-5xl">We Provide Quality</h1>
```

#### Hover Effects

```html
<!-- Hover color change -->
<a class="text-gray-700 hover:text-blue-600">Link</a>

<!-- Hover background change -->
<button class="bg-blue-600 hover:bg-blue-700">Button</button>

<!-- Hover scale (grow) -->
<div class="transform hover:scale-105">Hover to grow</div>

<!-- Hover shadow -->
<div class="shadow-md hover:shadow-lg">Hover for shadow</div>
```

### Modifying the Gradient Accent

Your page uses a special purple gradient for highlights:

**Location:** Lines 17-19 (in the `<style>` section)

```html
<style>
    .gradient-accent {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    }
</style>
```

This gradient goes from purple-blue (#667eea) to darker purple (#764ba2).

**To change the gradient colors:**
1. Find `.gradient-accent` in the style section
2. Replace the hex color codes (#667eea and #764ba2) with new colors

**Common hex color codes:**
- Blue: `#3b82f6`
- Green: `#10b981`
- Red: `#ef4444`
- Orange: `#f97316`
- Pink: `#ec4899`

**Example - Change to blue gradient:**
```html
.gradient-accent {
    background: linear-gradient(135deg, #3b82f6 0%, #1e40af 100%);
}
```

### Key Sections Using Tailwind Classes

#### Hero Section Styling

The hero section uses several Tailwind classes you might want to adjust:

```html
<section class="relative min-h-screen flex items-center justify-center">
    <!-- min-h-screen = full screen height -->
    <!-- flex = flexible layout -->
    <!-- items-center = vertically centered -->
    <!-- justify-center = horizontally centered -->
</section>
```

**To change hero section height:**
- `min-h-screen` = Full screen height (current)
- `min-h-96` = Fixed smaller height
- `py-20` = Specific padding top and bottom

#### Feature Cards

```html
<div class="hover-lift bg-gradient-to-br from-blue-50 to-indigo-50 rounded-xl p-8 border border-blue-100">
    <!-- hover-lift = custom animation on hover -->
    <!-- bg-gradient-to-br = gradient background (top-left to bottom-right) -->
    <!-- rounded-xl = rounded corners -->
    <!-- p-8 = padding inside -->
    <!-- border border-blue-100 = border styling -->
</div>
```

**To change card styling:**
- Change `from-blue-50 to-indigo-50` to different colors
- Change `rounded-xl` to `rounded-lg` for less rounded corners
- Change `p-8` to `p-6` or `p-10` for different padding

#### Button Styling

```html
<a href="..." class="bg-blue-600 text-white px-8 py-4 rounded-lg font-bold hover:bg-blue-700 transform hover:scale-105">
    Get Started
</a>
```

**To customize buttons:**
- Change `bg-blue-600` to different color
- Change `px-8 py-4` to adjust button size
- Change `rounded-lg` to `rounded-full` for pill-shaped button
- Remove `transform hover:scale-105` to remove grow effect on hover

---

## Fixing and Managing Links

### Understanding Links in HTML

A link is created with the `<a>` tag:

```html
<a href="https://www.example.com">Click here</a>
```

Breaking this down:
- `<a>` = Anchor tag (creates a link)
- `href="..."` = The URL the link goes to
- `Click here` = The text that appears as a link

### Types of Links in Your Landing Page

#### Internal Links (Links to sections on same page)

These use `#` followed by the section ID:

```html
<!-- Navigation link: -->
<a href="#features">Features</a>

<!-- Target section: -->
<section id="features">
    ...
</section>
```

When you click the link, the page scrolls to that section.

#### External Links (Links to other websites)

These use full URLs:

```html
<a href="https://www.handyman.com">Get Started</a>
```

#### Email Links

These use `mailto:`:

```html
<a href="mailto:john@handyman.com">Email Us</a>
```

#### Phone Links

These use `tel:`:

```html
<a href="tel:+1234567890">Call Now</a>
```

### All Links in Your Landing Page - Complete List

#### Navigation Menu Links

**Location:** Lines 50-57 (Desktop menu) and Lines 65-72 (Mobile menu)

```html
<!-- Desktop Navigation -->
<a href="#features" class="...">Features</a>
<a href="#benefits" class="...">Benefits</a>
<a href="#about" class="...">About</a>
<a href="#testimonials" class="...">Testimonials</a>
<a href="#faq" class="...">FAQ</a>
<a href="https://www.handyman.com" class="...">Get Started</a>
```

**Status:** 
- ✅ Internal links (#features, #benefits, etc.) are correct
- ⚠️ External link `https://www.handyman.com` needs to be updated

**To update the Get Started button:**
```html
<!-- Original: -->
<a href="https://www.handyman.com" class="...">Get Started</a>

<!-- Updated (example): -->
<a href="https://www.yourwebsite.com/booking" class="...">Get Started</a>
```

#### Hero Section CTA Buttons

**Location:** Lines 94-99

```html
<!-- Blue button: -->
<a href="https://www.handyman.com" class="...">Get Your Free Quote</a>

<!-- Outline button: -->
<a href="#features" class="...">Learn More</a>
```

**To update:**
1. Change `https://www.handyman.com` to your booking/quote page
2. The "Learn More" button is correct (goes to #features section)

#### CTA Section Buttons

**Location:** Lines 667-676

```html
<a href="https://www.handyman.com" class="...">Call Now for Free Quote</a>
<a href="mailto:john@handyman.com" class="...">Email Us</a>
```

**To update:**
1. Change `https://www.handyman.com` to your booking page
2. Change `john@handyman.com` to your actual email address

#### Footer Links

**Location:** Lines 720-850 (approximately)

**Quick Links Section:**
```html
<li><a href="#features" class="...">Features</a></li>
<li><a href="#benefits" class="...">Benefits</a></li>
<li><a href="#about" class="...">About Us</a></li>
<li><a href="#testimonials" class="...">Testimonials</a></li>
<li><a href="#faq" class="...">FAQ</a></li>
```

✅ These are all correct (internal links)

**Services Section:**
```html
<li><a href="#" class="...">Plumbing Repairs</a></li>
<li><a href="#" class="...">Electrical Work</a></li>
<li><a href="#" class="...">Carpentry</a></li>
<li><a href="#" class="...">Painting</a></li>
<li><a href="#" class="...">Installation</a></li>
```

⚠️ These links use `#` (placeholder). **Options:**
- Option 1: Create individual service pages and link to them
- Option 2: Create a services section on the page and link to it
- Option 3: Link to your main website

**Contact Information:**
```html
<a href="mailto:john@handyman.com" class="...">john@handyman.com</a>
<a href="tel:+1234567890" class="...">(123) 456-7890</a>
```

⚠️ These need to be updated with your actual contact info

**Policy Links (Bottom Footer):**
```html
<a href="privacy.html" class="...">Privacy Policy</a>
<a href="terms.html" class="...">Terms of Service</a>
<a href="blog.html" class="...">Blog</a>
<a href="https://www.handyman.com" class="...">Visit Website</a>
```

⚠️ These need attention:
- `privacy.html` - Needs to be created or path updated
- `terms.html` - Needs to be created or path updated
- `blog.html` - Optional, can be removed if not needed
- `https://www.handyman.com` - Update to your website

### Step-by-Step: Fix All Broken Links

#### Step 1: Update External Links

**Find and replace all instances of:**
`https://www.handyman.com`

**With your actual website URL:**
`https://www.yourwebsite.com`

**Locations to update:**
1. Line ~56: Navigation "Get Started" button
2. Line ~95: Hero "Get Your Free Quote" button
3. Line ~669: CTA "Call Now for Free Quote" button
4. Line ~847: Footer "Visit Website" link

**How to find them quickly:**
1. Use Ctrl+F (Cmd+F on Mac) to open Find
2. Search for `www.handyman.com`
3. Replace each occurrence with your URL

#### Step 2: Update Contact Information

**Find:**
```html
<a href="mailto:john@handyman.com">john@handyman.com</a>
<a href="tel:+1234567890">(123) 456-7890</a>
```

**Replace with your contact info:**
```html
<a href="mailto:your-email@yoursite.com">your-email@yoursite.com</a>
<a href="tel:+1234567890">Your Phone Number</a>
```

**Locations:**
- Line ~674: CTA section email link
- Lines ~810 & ~814: Footer contact information

#### Step 3: Update Service Links (Choose One Approach)

**Approach A - Link to external website (simplest):**
```html
<!-- Original: -->
<li><a href="#" class="...">Plumbing Repairs</a></li>

<!-- Updated: -->
<li><a href="https://www.yourwebsite.com/services" class="...">Plumbing Repairs</a></li>
```

**Approach B - Create internal service pages:**
```html
<!-- Create files: plumbing.html, electrical.html, etc. -->

<!-- Then update links: -->
<li><a href="plumbing.html" class="...">Plumbing Repairs</a></li>
<li><a href="electrical.html" class="...">Electrical Work</a></li>
```

**Approach C - Remove service links:**
```html
<!-- Delete the entire Services section from footer if not needed -->
```

#### Step 4: Update Social Media Links

**Location:** Lines 720-726 (Footer social icons)

```html
<a href="#" class="..."><i class="fab fa-facebook-f"></i></a>
<a href="#" class="..."><i class="fab fa-twitter"></i></a>
<a href="#" class="..."><i class="fab fa-instagram"></i></a>
<a href="#" class="..."><i class="fab fa-linkedin-in"></i></a>
```

**Update with your social media URLs:**
```html
<a href="https://www.facebook.com/yourpage" class="..."><i class="fab fa-facebook-f"></i></a>
<a href="https://www.twitter.com/yourhandle" class="..."><i class="fab fa-twitter"></i></a>
<a href="https://www.instagram.com/yourhandle" class="..."><i class="fab fa-instagram"></i></a>
<a href="https://www.linkedin.com/company/yourcompany" class="..."><i class="fab fa-linkedin-in"></i></a>
```

**Or remove if you don't use them:**
```html
<!-- Delete the entire social media section -->
```

### Link Verification Checklist

After updating links, verify them:

- [ ] All navigation menu links work
- [ ] "Get Started" buttons go to correct page
- [ ] Email links open email client with your address
- [ ] Phone links dial your number
- [ ] All footer links work
- [ ] Social media links go to your profiles
- [ ] Internal section links scroll to correct sections

---

## Linking Privacy and Terms Pages

### Why You Need Privacy and Terms Pages

These pages are important for:
- Legal compliance (especially GDPR, CCPA)
- Building customer trust
- Protecting your business
- Professional appearance

### Step 1: Create the Privacy Policy Page

**File name:** `privacy.html`

**Save location:** Same folder as your `index.html`

**Basic structure to start with:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Privacy Policy - John's Handyman">
    <title>Privacy Policy - John's Handyman</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-900">
    <!-- Header (same as index.html) -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <i class="fas fa-tools text-blue-600 text-2xl"></i>
                <h1 class="text-2xl font-bold text-gray-900">John's Handyman</h1>
            </div>
            <div class="hidden md:flex items-center gap-8">
                <a href="index.html" class="text-gray-700 font-medium hover:text-blue-600">Home</a>
                <a href="index.html#features" class="text-gray-700 font-medium hover:text-blue-600">Features</a>
                <a href="index.html#faq" class="text-gray-700 font-medium hover:text-blue-600">FAQ</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl font-bold text-gray-900 mb-8">Privacy Policy</h1>
            
            <div class="space-y-8 text-gray-700 leading-relaxed">
                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Introduction</h2>
                    <p>John's Handyman ("we," "our," or "us") is committed to protecting your privacy. This Privacy Policy explains how we collect, use, disclose, and safeguard your information when you visit our website.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Information We Collect</h2>
                    <p>We may collect information about you in a variety of ways. The information we may collect on the Site includes:</p>
                    <ul class="list-disc list-inside mt-4 space-y-2">
                        <li>Personal Data: Personally identifiable information, such as your name, shipping address, email address, and telephone number, that you voluntarily give to us when you register with the Site or when you choose to participate in various activities related to the Site.</li>
                        <li>Financial Data: Financial information, such as data related to your payment method (e.g., valid credit card number, card brand, expiration date) that we may collect when you purchase, order, return, exchange, or request information about our services from the Site.</li>
                        <li>Data From Forms: Any data we collect from you in custom forms you complete for your convenience.</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Use of Your Information</h2>
                    <p>Having accurate information about you permits us to provide you with a smooth, efficient, and customized experience. Specifically, we may use information collected about you via the Site to:</p>
                    <ul class="list-disc list-inside mt-4 space-y-2">
                        <li>Generate a personal profile about you so that future visits to the Site will be personalized as possible.</li>
                        <li>Increase the efficiency and operation of the Site.</li>
                        <li>Monitor and analyze usage and trends to improve your experience with the Site.</li>
                        <li>Notify you of updates to the Site.</li>
                        <li>Process your transactions and send you related information.</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Disclosure of Your Information</h2>
                    <p>We may share information we have collected about you in certain situations:</p>
                    <ul class="list-disc list-inside mt-4 space-y-2">
                        <li><strong>By Law or to Protect Rights:</strong> If we believe the release of information is necessary to comply with the law, enforce our Site policies, or protect ours or others' rights, property, or safety.</li>
                        <li><strong>Third-Party Service Providers:</strong> We may share your information with third parties that perform services for us or on our behalf, including payment processing, data analysis, email delivery, hosting services, and customer service.</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Security of Your Information</h2>
                    <p>We use administrative, technical, and physical security measures to protect your personal information. However, perfect security cannot be guaranteed on the Internet.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Contact Us</h2>
                    <p>If you have questions or comments about this Privacy Policy, please contact us at:</p>
                    <p class="mt-4">
                        <strong>John's Handyman</strong><br>
                        Email: john@handyman.com<br>
                        Phone: (123) 456-7890
                    </p>
                </div>

                <div class="pt-8 border-t">
                    <p class="text-sm text-gray-600">Last updated: January 2025</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer (same as index.html) -->
    <footer class="bg-gray-900 text-gray-300 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center pt-8 border-t border-gray-800">
                <p class="text-gray-400">&copy; 2025 John's Handyman. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Step 2: Create the Terms of Service Page

**File name:** `terms.html`

**Save location:** Same folder as your `index.html`

**Basic structure:**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Terms of Service - John's Handyman">
    <title>Terms of Service - John's Handyman</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        html {
            scroll-behavior: smooth;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-900">
    <!-- Header -->
    <header class="sticky top-0 z-50 bg-white shadow-md">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-4 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <i class="fas fa-tools text-blue-600 text-2xl"></i>
                <h1 class="text-2xl font-bold text-gray-900">John's Handyman</h1>
            </div>
            <div class="hidden md:flex items-center gap-8">
                <a href="index.html" class="text-gray-700 font-medium hover:text-blue-600">Home</a>
                <a href="index.html#features" class="text-gray-700 font-medium hover:text-blue-600">Features</a>
                <a href="index.html#faq" class="text-gray-700 font-medium hover:text-blue-600">FAQ</a>
            </div>
        </nav>
    </header>

    <!-- Main Content -->
    <section class="py-24 bg-white">
        <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
            <h1 class="text-4xl font-bold text-gray-900 mb-8">Terms of Service</h1>
            
            <div class="space-y-8 text-gray-700 leading-relaxed">
                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Agreement to Terms</h2>
                    <p>These Terms of Service ("Terms") constitute a legally binding agreement made between you, whether personally or on behalf of an entity ("you") and John's Handyman ("Company," "we," "us," or "our"), concerning your access to and use of the website as well as any other media form, media channel, mobile website, or mobile application relating, linked, or otherwise connected thereto (collectively, the "Site").</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Intellectual Property Rights</h2>
                    <p>Unless otherwise indicated, the Site is our proprietary property and all source code, databases, functionality, software, website designs, audio, video, text, photographs, and graphics on the Site (collectively, the "Content") and the trademarks, service marks, and logos contained therein (the "Marks") are owned or controlled by us or licensed to us, and are protected by copyright and trademark laws.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">User Representations</h2>
                    <p>By using the Site, you represent and warrant that:</p>
                    <ul class="list-disc list-inside mt-4 space-y-2">
                        <li>All registration information you submit is true, accurate, current, and complete.</li>
                        <li>You will maintain the confidentiality of your account and password.</li>
                        <li>You will maintain the accuracy of account information and promptly update such information.</li>
                        <li>You have the legal capacity and you agree to comply with these Terms of Service.</li>
                        <li>You are not a minor in the jurisdiction in which you reside.</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Prohibited Activities</h2>
                    <p>You may not access or use the Site for any purpose other than that for which we make the Site available. The Site may not be used in connection with any commercial endeavors except those specifically endorsed or approved by us.</p>
                    <p class="mt-4">As a user of the Site, you agree not to:</p>
                    <ul class="list-disc list-inside mt-4 space-y-2">
                        <li>Systematically retrieve data or other content from the Site to create or compile a collection, compilation, database, or directory without written permission from us.</li>
                        <li>Trick, defraud, or mislead us and other users, especially in any attempt to learn sensitive account information.</li>
                        <li>Circumvent, disable, or otherwise interfere with security-related features of the Site.</li>
                        <li>Disparage, tarnish, or otherwise harm, in our opinion, us and/or the Site.</li>
                    </ul>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Limitation of Liability</h2>
                    <p>In no event shall our company or its suppliers be liable for any damages (including, without limitation, damages for loss of data or profit, or due to business interruption) arising out of or in connection with the use or inability to use the materials on the Site.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Modifications and Interruptions</h2>
                    <p>We reserve the right to modify or discontinue, temporarily or permanently, the Site (or any part thereof) with or without notice. You agree that we will not be liable to you or to any third party for any modification, suspension, or discontinuance of the Site.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Governing Law</h2>
                    <p>These terms and conditions are governed by and construed in accordance with the laws of your jurisdiction, and you irrevocably submit to the exclusive jurisdiction of the courts in that location.</p>
                </div>

                <div>
                    <h2 class="text-2xl font-bold text-gray-900 mb-4">Contact Us</h2>
                    <p>If you have any questions about these Terms of Service, please contact us at:</p>
                    <p class="mt-4">
                        <strong>John's Handyman</strong><br>
                        Email: john@handyman.com<br>
                        Phone: (123) 456-7890
                    </p>
                </div>

                <div class="pt-8 border-t">
                    <p class="text-sm text-gray-600">Last updated: January 2025</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-gray-900 text-gray-300 py-16">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center pt-8 border-t border-gray-800">
                <p class="text-gray-400">&copy; 2025 John's Handyman. All rights reserved.</p>
            </div>
        </div>
    </footer>
</body>
</html>
```

### Step 3: Update Links in index.html

Now update your main page to link to these new pages.

**Location 1: Footer Policy Links (Line ~845)**

**Original:**
```html
<a href="privacy.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 flex items-center gap-2">
    <i class="fas fa-shield-alt"></i>
    Privacy Policy
</a>
<a href="terms.html" class="text-gray-400 hover:text-blue-400 transition-colors duration-300 flex items-center gap-2">
    <i class="fas fa-file-contract"></i>
    Terms of Service
</a>
```

✅ These links are already correct! They point to `privacy.html` and `terms.html` in the same folder.

**Just make sure:**
1. Your `privacy.html` file is in the same folder as `index.html`
2. Your `terms.html` file is in the same folder as `index.html`
3. The file names match exactly (case-sensitive on some servers)

### Step 4: Optional - Add Policy Links to Navigation

You can also add these links to your header navigation for easier access.

**Location:** Lines 50-57 (Desktop menu)

**Add before the "Get Started" button:**
```html
<a href="privacy.html" class="text-gray-700 font-medium hover:text-blue-600 transition-colors duration-300">Privacy</a>
<a href="terms.html" class="text-gray-700 font-medium hover:text-blue-600 transition-colors duration-300">Terms</a>
```

**Also add to mobile menu (Lines 65-72):**
```html
<a href="privacy.html" class="text-gray-700 font-medium hover:text-blue-600 transition-colors duration-300 py-2">Privacy</a>
<a href="terms.html" class="text-gray-700 font-medium hover:text-blue-600 transition-colors duration-300 py-2">Terms</a>
```

### Step 5: Customize Policy Content

The templates provided are generic. You should customize them with:

**In privacy.html:**
- Your actual business name
- Your actual email address
- Your actual phone number
- Your specific data collection practices
- Your specific data usage practices
- Your company's privacy practices

**In terms.html:**
- Your actual business name
- Your actual email address
- Your actual phone number
- Your specific terms and conditions
- Your warranty policies
- Your cancellation policies
- Your dispute resolution process

### File Structure After Setup

Your project folder should look like this:

```
your-project-folder/
├── index.html          (main landing page)
├── privacy.html        (privacy policy)
├── terms.html          (terms of service)
└── (optional) blog.html (blog page)
```

### Verification Checklist

- [ ] Created `privacy.html` file
- [ ] Created `terms.html` file
- [ ] Both files are in the same folder as `index.html`
- [ ] Footer links to privacy.html work
- [ ] Footer links to terms.html work
- [ ] (Optional) Navigation links to policies work
- [ ] All contact information is updated in policy pages
- [ ] Policy content is customized for your business

---

## Common Customization Tasks

### Task 1: Change the Hero Background

The hero section has animated gradient blobs in the background.

**Location:** Lines 119-121

```html
<div class="absolute top-0 right-0 w-96 h-96 bg-blue-200 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-pulse"></div>
<div class="absolute bottom-0 left-0 w-96 h-96 bg-indigo-200 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-pulse"></div>
```

**To change blob colors:**
- `bg-blue-200` → Change to any color class (bg-green-200, bg-purple-200, etc.)
- `bg-indigo-200` → Change to any color class

**To remove blobs entirely:**
Delete both `<div>` lines.

### Task 2: Add a New Feature Card

**Location:** After the existing feature cards (around line 230)

**Copy this template:**
```html
<div class="hover-lift bg-gradient-to-br from-red-50 to-orange-50 rounded-xl p-8 border border-red-100">
    <div class="w-16 h-16 bg-red-600 rounded-lg flex items-center justify-center mb-6">
        <i class="fas fa-fire text-white text-2xl"></i>
    </div>
    <h3 class="text-2xl font-bold text-gray-900 mb-4">Your Feature Title</h3>
    <p class="text-gray-700 mb-4">Your feature description goes here. Explain the benefit to customers.</p>
    <ul class="space-y-2 text-gray-600">
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-600"></i>
            <span>Benefit point 1</span>
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-600"></i>
            <span>Benefit point 2</span>
        </li>
        <li class="flex items-center gap-2">
            <i class="fas fa-check text-green-600"></i>
            <span>Benefit point 3</span>
        </li>
    </ul>
</div>
```

**Customize:**
1. Change `from-red-50 to-orange-50` to your desired gradient colors
2. Change `bg-red-600` to match the gradient colors
3. Change the icon: `fa-fire` to any Font Awesome icon
4. Update title, description, and bullet points
5. Add to the grid in the Features section

### Task 3: Add a New FAQ Item

**Location:** After the last FAQ item (around line 650)

**Copy this template:**
```html
<div class="faq-item bg-gray-50 rounded-lg border border-gray-200 overflow-hidden">
    <button class="faq-question w-full px-6 py-4 text-left flex items-center justify-between hover:bg-gray-100 transition-colors duration-300 cursor-pointer">
        <span class="text-lg font-semibold text-gray-900">Your Question Here?</span>
        <i class="faq-icon fas fa-chevron-down text-gray-600 transition-transform duration-300"></i>
    </button>
    <div class="faq-answer hidden px-6 py-4 bg-white border-t border-gray-200">
        <p class="text-gray-700 leading-relaxed">Your answer goes here. Provide a clear, helpful response to the question.</p>
    </div>
</div>
```

**Customize:**
1. Replace "Your Question Here?" with your question
2. Replace the answer text with your response
3. Add to the FAQ section

### Task 4: Change the Color Scheme

To change the overall color scheme from blue/purple to a different color:

**Step 1: Update the gradient accent**
Location: Lines 17-19
```html
.gradient-accent {
    background: linear-gradient(135deg, #NEW-COLOR-1 0%, #NEW-COLOR-2 100%);
}
```

**Step 2: Replace all blue classes**
Search for: `bg-blue-` and `text-blue-`
Replace with: `bg-green-` or `bg-purple-` or your chosen color

**Step 3: Update button colors**
Find all: `class="bg-blue-600 ... hover:bg-blue-700"`
Replace with: `class="bg-[your-color]-600 ... hover:bg-[your-color]-700"`

**Example color combinations:**
- Green: `#10b981` and `#059669`
- Purple: `#a855f7` and `#7e22ce`
- Red: `#ef4444` and `#dc2626`
- Orange: `#f97316` and `#ea580c`

### Task 5: Add or Remove Sections

**To remove a section:**
1. Find the section (e.g., `<section id="benefits">`)
2. Delete the entire section from opening `<section>` to closing `</section>`
3. Remove the navigation link to that section

**To add a new section:**
1. Copy an existing section as a template
2. Modify the content
3. Add a navigation link to it
4. Give it a unique `id` attribute

### Task 6: Update Hero Section Image

The About section has a background image:

**Location:** Line ~385

```html
<img src="https://images.unsplash.com/photo-1504328345606-18bbc8c9d7d1?w=600&h=400&fit=crop" alt="Professional handyman at work" class="w-full h-96 object-cover opacity-90">
```

**To change the image:**
1. Find a new image URL from Unsplash, Pexels, or Pixabay
2. Replace the entire `src` URL
3. Update the `alt` text to describe the new image

**Example:**
```html
<img src="https://images.unsplash.com/photo-1581092918056-0c4c3acd3789?w=600&h=400&fit=crop" alt="Home renovation project" class="w-full h-96 object-cover opacity-90">
```

### Task 7: Change Button Text and Links

**Find any button:**
```html
<a href="..." class="...">Button Text</a>
```

**Update:**
1. Change `Button Text` to new text
2. Change `href="..."` to new link

**Example:**
```html
<!-- Original: -->
<a href="https://www.handyman.com" class="...">Get Your Free Quote</a>

<!-- Updated: -->
<a href="https://calendly.com/yourname" class="...">Book an Appointment</a>
```

---

## Troubleshooting Guide

### Problem: Links Don't Work

**Symptoms:**
- Clicking a link does nothing
- Page shows 404 error
- Link goes to wrong page

**Solutions:**

1. **Check the file name:**
   - Make sure `privacy.html` and `terms.html` exist in the same folder
   - File names are case-sensitive on some servers
   - Correct: `privacy.html` ❌ Wrong: `Privacy.html` or `privacy.HTML`

2. **Check the URL format:**
   ```html
   <!-- For files in same folder: -->
   <a href="privacy.html">Privacy</a>  ✅ Correct
   
   <!-- For external URLs: -->
   <a href="https://www.example.com">Link</a>  ✅ Correct
   
   <!-- For email: -->
   <a href="mailto:email@example.com">Email</a>  ✅ Correct
   ```

3. **Verify the href attribute:**
   ```html
   <!-- ❌ Wrong - missing href -->
   <a class="...">Link</a>
   
   <!-- ✅ Correct -->
   <a href="page.html" class="...">Link</a>
   ```

4. **Check for typos:**
   - `www.handyman.com` vs `www.handyman.co`
   - `john@handyman.com` vs `john@handyman.com` (spacing issues)

### Problem: Styling Looks Wrong

**Symptoms:**
- Colors are different than expected
- Text is too large or too small
- Spacing is wrong
- Elements overlap

**Solutions:**

1. **Clear browser cache:**
   - Press Ctrl+Shift+R (Cmd+Shift+R on Mac) to hard refresh
   - This reloads the page without using cached version

2. **Check Tailwind classes:**
   ```html
   <!-- ❌ Wrong - class name typo -->
   <div class="bg-blue-60 p-4">Wrong</div>
   
   <!-- ✅ Correct -->
   <div class="bg-blue-600 p-4">Correct</div>
   ```

3. **Verify class combinations:**
   - Don't mix conflicting classes
   - Example: `text-left` and `text-center` together won't work

4. **Check for missing closing tags:**
   ```html
   <!-- ❌ Wrong - missing closing </div> -->
   <div class="...">
       <p>Content</p>
   
   <!-- ✅ Correct -->
   <div class="...">
       <p>Content</p>
   </div>
   ```

### Problem: Mobile Menu Doesn't Work

**Symptoms:**
- Mobile menu button doesn't toggle
- Menu stays hidden or always visible
- Menu icon doesn't change

**Solutions:**

1. **Check JavaScript section:**
   - Make sure the JavaScript code at the bottom is intact
   - Look for any error messages in browser console (F12 → Console tab)

2. **Verify mobile menu HTML:**
   ```html
   <!-- Should exist in header: -->
   <button class="md:hidden mobile-menu-button">
       <i class="fas fa-bars"></i>
   </button>
   
   <div class="mobile-menu hidden">
       <!-- Menu items -->
   </div>
   ```

3. **Check class names match:**
   - JavaScript looks for `.mobile-menu-button` class
   - Make sure button has this exact class name
   - Make sure menu div has `.mobile-menu` class

### Problem: Images Don't Show

**Symptoms:**
- Image placeholder shows instead of image
- Broken image icon appears
- No image visible

**Solutions:**

1. **Check image URL:**
   ```html
   <!-- ❌ Wrong - broken URL -->
   <img src="https://images.unsplash.com/broken-url">
   
   <!-- ✅ Correct - valid URL -->
   <img src="https://images.unsplash.com/photo-1504328345606-18bbc8c9d7d1?w=600">
   ```

2. **Verify alt text:**
   ```html
   <!-- ✅ Always include alt text -->
   <img src="..." alt="Descriptive text for image">
   ```

3. **Check image permissions:**
   - Make sure you have rights to use the image
   - Use free image sites: Unsplash, Pexels, Pixabay
   - Check if image URL is still active

### Problem: Text Content Not Updating

**Symptoms:**
- Changes don't appear when you refresh
- Old text still shows
- New text doesn't show

**Solutions:**

1. **Save the file:**
   - Make sure you saved after editing (Ctrl+S or Cmd+S)
   - Check the file was actually saved

2. **Hard refresh the page:**
   - Ctrl+Shift+R (Cmd+Shift+R on Mac)
   - This forces the browser to reload everything

3. **Check you're editing the right file:**
   - Make sure you're editing `index.html`
   - Not a backup or copy of the file

4. **Verify changes were saved:**
   - Look for unsaved indicator (usually a dot or asterisk in editor)
   - Make sure file shows correct content when you reopen it

### Problem: Spacing or Layout Broken

**Symptoms:**
- Elements overlap
- Too much or too little space
- Layout looks misaligned

**Solutions:**

1. **Check for missing closing tags:**
   ```html
   <!-- ❌ Wrong - content outside intended container -->
   <div class="p-8">
       <h1>Title</h1>
   </div> <!-- Missing closing tag above -->
   <p>This paragraph is outside the div</p>
   
   <!-- ✅ Correct -->
   <div class="p-8">
       <h1>Title</h1>
       <p>This paragraph is inside the div</p>
   </div>
   ```

2. **Verify Tailwind spacing classes:**
   - `p-4` = padding inside (16px)
   - `m-4` = margin outside (16px)
   - `gap-4` = space between items (16px)

3. **Check responsive classes:**
   - Make sure you're testing on correct screen size
   - Mobile: less than 640px
   - Tablet: 640px - 1024px
   - Desktop: 1024px and up

### Problem: FAQ Accordion Doesn't Work

**Symptoms:**
- Clicking questions doesn't expand answers
- All answers show at once
- No animation when clicking

**Solutions:**

1. **Verify JavaScript is present:**
   - Check the `<script>` section at the bottom of the page exists
   - Look for FAQ accordion code

2. **Check FAQ structure:**
   ```html
   <!-- ✅ Correct structure -->
   <div class="faq-item">
       <button class="faq-question">
           <span>Question?</span>
           <i class="faq-icon fas fa-chevron-down"></i>
       </button>
       <div class="faq-answer hidden">
           <p>Answer</p>
       </div>
   </div>
   ```

3. **Verify class names:**
   - `.faq-item` - wrapper
   - `.faq-question` - clickable button
   - `.faq-answer` - answer container
   - `.faq-icon` - chevron icon
   - `hidden` - class for hidden state

### Problem: Colors Look Different Than Expected

**Symptoms:**
- Gradient colors are wrong
- Button colors don't match
- Text colors are incorrect

**Solutions:**

1. **Check Tailwind color values:**
   - Tailwind uses specific color names and numbers
   - `blue-600` is different from `blue-700`
   - Reference: [Tailwind Colors](https://tailwindcss.com/docs/customizing-colors)

2. **Verify gradient syntax:**
   ```html
   <!-- ❌ Wrong -->
   background: linear-gradient(#667eea, #764ba2);
   
   <!-- ✅ Correct -->
   background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
   ```

3. **Check for conflicting classes:**
   - Only one background color class should apply
   - Example: Don't use both `bg-blue-600` and `bg-green-600`

### Problem: Page Looks Different on Mobile

**Symptoms:**
- Layout breaks on phone
- Text is too large or small
- Elements overlap on mobile

**Solutions:**

1. **Test responsive design:**
   - Open page in browser
   - Press F12 to open Developer Tools
   - Click mobile device icon to test different screen sizes

2. **Check responsive classes:**
   ```html
   <!-- ✅ Good - different sizes for different screens -->
   <h1 class="text-2xl sm:text-3xl md:text-4xl lg:text-5xl">
       Responsive heading
   </h1>
   ```

3. **Verify viewport meta tag:**
   ```html
   <!-- ✅ Should be in <head> section -->
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
   ```

### Getting Help

If you encounter an issue not covered above:

1. **Check browser console for errors:**
   - Press F12 to open Developer Tools
   - Go to Console tab
   - Look for red error messages

2. **Validate HTML:**
   - Visit [W3C HTML Validator](https://validator.w3.org/)
   - Paste your HTML code
   - Look for errors

3. **Common resources:**
   - [Tailwind CSS Documentation](https://tailwindcss.com/docs)
   - [Font Awesome Icons](https://fontawesome.com/icons)
   - [HTML/CSS Reference](https://developer.mozilla.org/en-US/)

---

## Final Checklist Before Launch

Use this checklist before making your page live:

### Content Updates
- [ ] Business name updated everywhere
- [ ] All contact information correct
- [ ] All links updated and tested
- [ ] Meta tags updated (title, description, keywords)
- [ ] Social media links added or removed
- [ ] All text proofread for typos

### Links & Navigation
- [ ] All internal links work (#features, #benefits, etc.)
- [ ] All external links work (website, booking page)
- [ ] Email links work (mailto:)
- [ ] Phone links work (tel:)
- [ ] Privacy policy page created and linked
- [ ] Terms of service page created and linked
- [ ] Mobile menu works on all devices

### Design & Styling
- [ ] Page looks good on mobile (< 640px)
- [ ] Page looks good on tablet (640-1024px)
- [ ] Page looks good on desktop (> 1024px)
- [ ] All colors are correct
- [ ] All fonts are readable
- [ ] No broken images
- [ ] No overlapping elements

### Functionality
- [ ] FAQ accordion works
- [ ] Mobile menu toggle works
- [ ] Smooth scrolling works
- [ ] All buttons clickable
- [ ] Form submissions work (if applicable)

### Performance
- [ ] Page loads quickly
- [ ] Images are optimized
- [ ] No console errors (F12 → Console)
- [ ] Page passes HTML validation

### SEO & Metadata
- [ ] Page title is descriptive
- [ ] Meta description is complete
- [ ] Keywords are relevant
- [ ] Alt text on all images
- [ ] Headings are properly structured (H1, H2, H3)

### Browser Compatibility
- [ ] Works in Chrome
- [ ] Works in Firefox
- [ ] Works in Safari
- [ ] Works in Edge

---

## Conclusion

You now have a comprehensive guide to maintaining and customizing your John's Handyman landing page. Remember:

1. **Always save your changes** (Ctrl+S or Cmd+S)
2. **Test on multiple devices** (mobile, tablet, desktop)
3. **Hard refresh your browser** (Ctrl+Shift+R) to see changes
4. **Keep backups** of your original files
5. **Test all links** before launching

For additional support, refer to:
- Tailwind CSS documentation
- Font Awesome icons library
- HTML/CSS tutorials
- Your web hosting provider's support

Good luck with your handyman service website!