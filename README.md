microlight.js
=============

*Note: This is a fork to add css based selection, view the original at https://github.com/asvd/microlight*

*microlight.js* is a micro-library (2.2k minified) which improves
 readability of code snippets by highlighting, for any programming
 language, yet without attaching additional language packages:

![preview]
(https://raw.githubusercontent.com/lopeax/microlight/css-based/microlight.PNG)

For a demo refer to http://codepen.io/zephyr/pen/MewjYd

## Installation

This library is installable by either npm or bower

--
**NPM**
```bash
npm i microlight-css-selection
```

--
**Bower**
```bash
bower install microlight-css-selection
```

## CSS

The following are some recommended css rules to target the elements within microlight

```css
.microlight {
    font-family: monospace;
    white-space: pre;
    background-color: #263238;
    color: #AABBC3;
    padding: 15px;
    text-align: left;
    overflow-x: auto;
    box-shadow: 0 2px 3px rgba(0,0,0,0.5);
    border-radius: 0.2em;
}

.microlight:not(:last-child) {
    margin-bottom: 15px;
}

// Colours inspired by https://atom.io/themes/atom-material-syntax
.microlight span[data_microlight_type="not-formatted"] {
    color: #B2CCD6;
}

.microlight span[data_microlight_type="keywords"] {
    color: #F1E655;
}

.microlight span[data_microlight_type="punctuation"] {
    color: #d9f5dd;
}

.microlight span[data_microlight_type="strings-regex"] {
    color: #C3E88D;
}

.microlight span[data_microlight_type="comments"] {
    color: #49656f;
}
```
