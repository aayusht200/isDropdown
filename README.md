# isDropdown

[![npm version](https://img.shields.io/npm/v/@aayusht200/isdropdown.svg)](https://www.npmjs.com/package/@aayusht200/isdropdown)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A simple, dependency-free JavaScript utility to enable dropdown toggling behavior for your UI.

---

## Installation

Using npm:

```bash
npm i @aayusht200/isdropdown
```

---

## Usage

Add required data attributes to your HTML:

```html
<div data-dropdown>
  <button data-dropdown-button>Toggle Dropdown</button>
  <div class="dropdown-content">
    <!-- Dropdown content here -->
  </div>
</div>
```

Then, use the package in your JavaScript:

```javascript
import { isDropdown } from '@aayusht200/isdropdown';

// Initialize dropdown toggle behavior
isDropdown();
```

Or with a standard `<script>` tag:

```html
<script src="path/to/isDropdown.js"></script>
<script>
  isDropdown();
</script>
```

---

## How it Works

- Assign `[data-dropdown]` to the wrapper containing your dropdown content.
- Assign `[data-dropdown-button]` to the button within that wrapper which opens/closes the dropdown.

Clicking the button toggles the `'active'` class on your `[data-dropdown]` element.  
Clicking elsewhere closes any open dropdowns.

### Example CSS

```css
[data-dropdown] .dropdown-content {
  display: none;
}

[data-dropdown].active .dropdown-content {
  display: block;
}
```

---

## API

### `isDropdown()`

- Initializes the dropdown logic on the document.
- No parameters needed.

---

## License

MIT

---

**NPM:** [@aayusht200/isdropdown](https://www.npmjs.com/package/@aayusht200/isdropdown)  
**GitHub:** [aayusht200/isDropdown](https://github.com/aayusht200/isDropdown)
