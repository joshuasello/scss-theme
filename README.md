# Scss Theme Module

## Installation

Clone this repository into your `scss` directory as `theme`.

```bash
cd /<path-to-scss-directory>/
git clone https://github.com/joshuasello/scss-theme.git theme
```

## Setup

### Expected directory structure

```text
scss/
    theme/
        ...
    home-page.scss
    ...  
```

## Importing

Importing as is:
```scss
// File: home-page.scss

@use "theme";

// The rest of your code...
```

Importing with changes to the default variables:
```scss
// File: home-page.scss

@use "theme" with (
  $primary-color: blue,
  $secondary-color: red
);

// The rest of your code...
```

## Colors

### SCSS Variables

- `$primary-color`
- `$secondary-color`
- `$tertiary-color`
- `$success-color`
- `$danger-color`
- `$warning-color`
- `$info-color`
- `$lightest-grey`
- `$light-grey`
- `$medium-grey`
- `$dark-grey`
- `$darkest-grey`


### CSS Variables

Color variables are also embedded as css variables so that they can be accessed by other running css or js processes.

CSS Example:
```css
a { color: var(--color-primary); }
p { color: var(--color-dark-grey); }
```
Javascript Example:
```js
console.log( getComputedStyle(document.body).getPropertyValue('--color-primary') )
```

### Color Helper Classes

- `.text-color-<color-name>` such as `.text-color-primary` or `.text-color-dark-grey`

## Shadows

### SCSS Variables
- `$light-shadow`
- `$medium-shadow`
- `$dark-shadow`

## Typography

### SCSS Variables
- `$heading-font-family`
- `$paragraph-font-family`
- `$quote-font-family`
- `$code-font-family`
- `$h1-size`
- `$h2-size`
- `$h3-size`
- `$h4-size`
- `$h5-size`
- `$h6-size`
- `$p-size`
- `$code-size`
- `$quote-size`

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## Authors
- Joshua Sello (joshuasello@gmail.com)

## License
[MIT](https://choosealicense.com/licenses/mit/)