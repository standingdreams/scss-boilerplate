# SCSS Boilerplate
Starting point for projects using SCSS.

## Requirements
- [Normalize.css](https://necolas.github.io/normalize.css/)
- Understanding of BEM

## Directories (In Cascading order)
- /configs
- /layouts
- /elements
- /components
- /pages
- /utilities

### Configs
Contains core styling for site. Normalizes styling by importing normalize via NPM. (Note: Normalize.css must be a dependency in project.) Base styling, breakpoints, mixing, variables and colors are defined here.

### Layouts
Contains all global layout element styling that are repeated throughout the site.

### Elements
Contains styling of all HTML tags. No HTML tag should receive site styling unless it is a global reset. All tags should receive a style unless they are nested inside of a component. If nested in a component, the tag can be styled inside of the component's class.

### Components
Contains partials that pertain to components within the site. Note: Be mindful of modifiers and usage throughout the site.

### Pages
Contains styling for each individual page. This directory should be used sparingly. Please try to use modifier classes on components first and resort to this if all else fails. It should override all other directories except for utilities. 

### Utilities
Contains override classes that are applied directly to the HTML element. This directory should be last so that it overrides all styling.