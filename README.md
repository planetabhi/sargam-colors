# Sargam Colors

Colors for designing warm, welcoming, caring sites and applications.

## Install

Install the package as a development dependency:

```shell-session
$ npm install @sargamdesign/colors --save-dev
```

## Usage

Import the stylesheet at the top of your CSS or SCSS file:

```css
@import "@sargamdesign/colors";
```

Set the `color-scheme` attribute on the HTML wrapper element to apply a theme. The following example applies the light theme:

```html
<html color-scheme="light">
```

To apply the dark theme, set the attribute to `dark`:

```html
<html color-scheme="dark">
```

## Color scales

The library provides seven color scales. Each step grows darker as the number increases. The following table lists each scale and its variables:

| Scale | Steps | Variables |
| --- | --- | --- |
| Red | 8 | `--red1` to `--red8` |
| Yellow | 8 | `--yellow1` to `--yellow8` |
| Green | 8 | `--green1` to `--green8` |
| Teal | 8 | `--teal1` to `--teal8` |
| Lavender | 8 | `--lavender1` to `--lavender8` |
| Pink | 8 | `--pink1` to `--pink8` |
| Silver | 10 | `--silver1` to `--silver10` |

## Semantic tokens

Semantic tokens map to theme-appropriate colors when you set the `color-scheme` attribute. The following table lists each token and its purpose:

| Token | Purpose |
| --- | --- |
| `--background` | Primary page background |
| `--background-subtle` | Background for raised surfaces |
| `--background-selected` | Background for selected elements |
| `--border-muted` | Low-contrast borders |
| `--border-default` | Default borders |
| `--border-strong` | High-contrast borders |
| `--content-primary` | Primary text |
| `--content-primary-alt` | Alternate primary text |
| `--content-secondary` | Secondary text |
| `--content-placeholder` | Placeholder text |
| `--link` | Link text |
| `--link-hover` | Link text in the hover state |
| `--link-subtle` | Low-emphasis link text |
| `--link-visited` | Visited link text |

Apply any token with the CSS `var()` function. The following example sets the text and background colors of a button:

```css
.button {
    color: var(--content-primary);
    background: var(--background-subtle);
}
```