# Premier Roofing Landing Page - Maintenance Guide

This guide provides detailed instructions for maintaining and customizing the Premier Roofing landing page. Whether you're new to web development or need a quick reference, you'll find step-by-step guidance for common updates.

## Table of Contents
1. [Updating Text and Tailwind CSS Classes](#updating-text-and-tailwind-css-classes)
2. [Fixing Broken Links](#fixing-broken-links)
3. [Linking Privacy and Terms Pages](#linking-privacy-and-terms-pages)
4. [Troubleshooting](#troubleshooting)

## Updating Text and Tailwind CSS Classes

### Header Section
```html
<div class="text-2xl font-bold text-gray-800">
    Premier Roofing
</div>
```
To update the company name:
1. Locate this div in the header section
2. Replace "Premier Roofing" with your desired text
3. Adjust text size using these Tailwind classes:
   - `text-xl` (smaller)
   - `text-2xl` (current size)
   - `text-3xl` (larger)

### Hero Section
```html
<h1 class="text-4xl md:text-5xl lg:text-6xl font-bold text-gray-900 leading-tight mb-8">
    Calgary's Premier Roofing Contractor
</h1>
```
To modify the main headline:
1. Replace the text between the `<h1>` tags
2. The current classes ensure responsive text sizing:
   - `text-4xl`: Mobile devices
   - `md:text-5xl`: Medium screens
   - `lg:text-6xl`: Large screens

### Features Section
Each feature card follows this structure:
```html
<div class="bg-white rounded-xl p-8 shadow-lg hover:shadow-xl transition-shadow duration-300">
    <h3 class="text-xl font-semibold mb-4">Ethical Practices</h3>
    <p class="text-gray-600 leading-relaxed">We maintain the highest standards...</p>
</div>
```
To update feature cards:
1. Locate the features section (`id="features"`)
2. Modify the `<h3>` text for the feature title
3. Update the `<p>` text for the description
4. Key styling classes:
   - `shadow-lg`: Default shadow
   - `hover:shadow-xl`: Shadow on hover
   - `rounded-xl`: Rounded corners

## Fixing Broken Links

### Navigation Menu Links
Current navigation structure:
```html
<div class="hidden md:flex space-x-8">
    <a href="#features" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Features</a>
    <a href="#benefits" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Benefits</a>
    <a href="#faq" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">FAQ</a>
    <a href="#contact" class="text-gray-600 hover:text-gray-900 transition-colors duration-300">Contact</a>
</div>
```
To update navigation links:
1. Locate the `href` attribute in each `<a>` tag
2. For internal page sections, use `#section-id`
3. For external links, use the full URL: `https://example.com`
4. Remember to update both desktop and mobile navigation menus

### Call-to-Action Links
```html
<a href="https://calgaryspremierroofer.com" class="inline-block bg-blue-600 text-white px-8 py-4 rounded-lg">
    Get Your Free Quote
</a>
```
To update CTA links:
1. Replace the `href` value with your desired URL
2. Test the link to ensure it opens correctly
3. Maintain the existing classes for consistent styling

## Linking Privacy and Terms Pages

### Footer Legal Links
Current structure:
```html
<div>
    <h3 class="text-white text-lg font-semibold mb-4">Legal</h3>
    <ul class="space-y-2">
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
        <li><a href="#" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
    </ul>
</div>
```
To add privacy and terms pages:
1. Create your privacy.html and terms.html files
2. Update the href attributes:
```html
<li><a href="privacy.html" class="text-gray-400 hover:text-white transition-colors duration-300">Privacy Policy</a></li>
<li><a href="terms.html" class="text-gray-400 hover:text-white transition-colors duration-300">Terms of Service</a></li>
```

## Troubleshooting

### Common Issues

1. **Broken Internal Links**
   - Ensure section IDs match the href values
   - Check for typos in IDs and href attributes
   - IDs are case-sensitive

2. **Responsive Design Issues**
   - Check that you've maintained the responsive classes:
     - `md:` prefix for medium screens
     - `lg:` prefix for large screens
   - Test on multiple screen sizes

3. **Styling Inconsistencies**
   - Keep the existing Tailwind classes when updating content
   - Use the same color classes (e.g., `text-gray-600`, `bg-blue-600`)
   - Maintain hover states with `hover:` classes

### Need Help?
- Review the [Tailwind CSS documentation](https://tailwindcss.com/docs)
- Test all changes in multiple browsers
- Keep a backup of the original code before making changes
- Use browser developer tools to inspect elements

Remember to test all changes thoroughly before deploying to production.