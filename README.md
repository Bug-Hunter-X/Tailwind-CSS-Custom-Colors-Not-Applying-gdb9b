# Tailwind CSS Custom Colors Not Applying Bug

This repository demonstrates a common issue with Tailwind CSS where custom colors defined in the `tailwind.config.js` file are not applied correctly. The problem is that the custom color `custom-color` is not being applied to the div element, even though the configuration appears correct.

## Bug Description

The `tailwind.config.js` file correctly defines the custom color `custom-color`, but the div element in `index.html` does not render with this color.  The issue is likely related to how Tailwind processes the configuration or the way the custom color is referenced. 

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies (if any).
3. Open `index.html` in a browser. 
4. Observe that the div element does not have the expected background color.

## Solution

The solution involves ensuring that Tailwind correctly processes the custom color by properly configuring the `content` array in `tailwind.config.js`. This array must include all files that use Tailwind CSS classes to allow the preprocessor to properly scan the files and include the styles from `tailwind.config.js`.