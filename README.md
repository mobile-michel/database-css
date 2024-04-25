# Simple template with Eleventy, Liquid & CDN css frameworks

## Folder structure

- templates in /content
- layouts in /_layouts
- includes in /_includes with /components
- JSON files in /_data
- SASS files in /sass
- images & JS in /assets with /admin (Decap CMS)

## Page layout

- _layouts/base.liquid: head code + DecapCMS scripts
- _layouts/default.liquid: HTML5 structure
- _includes/navPrimary.liquid with primary navigation
- _includes/searchSite.liquid to include in header landmark
- _includes/navSecondary.liquid with secondary navigation
- _includes/navFooter.liquid with footer navigation
- _includes/copyright.liquid to include in footer landmark
- _includes/subscribe.liquid to include in footer landmark

## Responsive navbar

- tags: add primary, secondary or footer in frontmatter

## Package.json scripts
- "start": "npx @11ty/eleventy --serve",
- "build": "eleventy"

## Dependencies
- "@11ty/eleventy": "^2.0.1"
- ready for [Decap CMS](https://decapcms.org/) integration.

## eleventy.config.js
```
module.exports = function (eleventyConfig) {
    eleventyConfig.addPassthroughCopy("./assets");
    return {
        dir: {
            input: "content", // Set the source for 11ty
            layouts: "../_layouts", // Base page layouts
            includes: "../_includes", // All UI partials
            data: "../_data", // JSON datasets
            output: "_site" // This is the default
        }
    };
};
```