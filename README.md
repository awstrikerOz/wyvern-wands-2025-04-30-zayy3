# Wyvern Wands Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Wyvern Wands landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step guidance for common maintenance tasks.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
The header contains your brand name and navigation menu. To update:

```html
<!-- Original -->
<a href="/" class="text-2xl font-bold text-gray-900">Wyvern Wands</a>

<!-- Example modification -->
<a href="/" class="text-2xl font-bold text-gray-900">Your Brand Name</a>
```

#### Key Tailwind Classes Explained:
- `text-2xl`: Sets large text size
- `font-bold`: Makes text bold
- `text-gray-900`: Sets dark gray text color

### Hero Section
The main banner section includes your headline and call-to-action:

```html
<h1 class="text-4xl md:text-6xl font-bold mb-6">Wyvern Wands</h1>
<p class="text-xl md:text-2xl mb-8">Handmade Wooden Wands</p>
```

To modify:
1. Change text between the opening and closing tags
2. Maintain the responsive classes (`md:text-6xl` means larger text on medium screens)
3. Keep the margin classes (`mb-6` adds bottom margin)

### Features Section
Each feature card follows this structure:

```html
<div class="bg-white p-8 rounded-xl shadow-lg hover:shadow-xl transition-shadow duration-300">
    <div class="text-center">
        <h3 class="text-xl font-semibold mb-4">Real Wood</h3>
        <p class="text-gray-600">Crafted from premium, sustainably sourced wood varieties</p>
    </div>
</div>
```

To update:
1. Locate the feature card you want to modify
2. Change the `<h3>` title text
3. Update the description in the `<p>` tag
4. Maintain the existing classes for consistent styling

## Fixing Broken Links

### Navigation Menu Links
Current placeholder links in the navigation:

```html
<div class="hidden md:flex space-x-8">
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors">Shop</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors">About</a>
    <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors">Contact</a>
</div>
```

To update links:
1. Replace `#` with your actual page URLs
2. Example:
```html
<a href="/shop.html" class="text-gray-600 hover:text-gray-900 transition-colors">Shop</a>
```

### Footer Links
The footer contains multiple link sections:

```html
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Shop</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">About</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Contact</a></li>
</ul>
```

Update these links to match your navigation menu links for consistency.

## Linking Privacy and Terms Pages

### Footer Policy Links
Locate the policies section in the footer:

```html
<!-- Original -->
<ul class="space-y-2">
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
    <li><a href="#" class="text-gray-400 hover:text-white transition-colors">Shipping Policy</a></li>
</ul>

<!-- Updated version -->
<ul class="space-y-2">
    <li><a href="/privacy.html" class="text-gray-400 hover:text-white transition-colors">Privacy Policy</a></li>
    <li><a href="/terms.html" class="text-gray-400 hover:text-white transition-colors">Terms of Service</a></li>
    <li><a href="/shipping.html" class="text-gray-400 hover:text-white transition-colors">Shipping Policy</a></li>
</ul>
```

## Troubleshooting

### Common Issues and Solutions

1. **Broken Layout After Text Changes**
   - Check that you haven't removed any closing tags
   - Verify all Tailwind classes remain intact
   - Ensure responsive classes (starting with `md:`) are preserved

2. **Links Not Working**
   - Confirm file paths are correct
   - Check for typos in URLs
   - Verify files exist in the specified locations

3. **Images Not Loading**
   - Ensure image paths are correct
   - Verify image files exist
   - Check image URL accessibility if using external sources

### Best Practices

1. Always backup files before making changes
2. Test changes in multiple browsers
3. Check responsive design using browser dev tools
4. Maintain consistent spacing and formatting
5. Keep original class structures intact when modifying content

Need additional help? Contact your web development team or refer to the [Tailwind CSS documentation](https://tailwindcss.com/docs).