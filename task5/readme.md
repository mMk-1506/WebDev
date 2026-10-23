# Laundry Services Hero Section

## 1. Project Description
This project involves designing a hero section for a laundry services website using HTML, CSS, and basic JavaScript. The webpage contains a navigation bar and a hero section with a heading, description, booking button, and laundry-related image.

## 2. Features
- Navigation bar with Logo, Home, Services, About Us, Contact Us, and Username.
- Hero section containing a heading, description, and booking button.
- Laundry-related image displayed beside the text.
- Hover effects on navigation links and the booking button.
- Viewport-based sizing and spacing.
- Simple JavaScript interaction for the booking button.

## 3. CSS Concepts

### A. CSS Display
The `display` property specifies how an element is displayed on a webpage.

Common values:
- `block`: Starts on a new line and generally occupies the available width.
- `inline`: Displays elements in the same line; width and height cannot normally be set directly.
- `inline-block`: Displays elements on the same line while allowing width and height to be specified.
- `none`: Hides the element and removes its layout space.

**Project usage:** `display: inline-block` is used to place the navigation items and hero content side by side without Flexbox.

### B. CSS Position
The `position` property controls how an element is positioned on a webpage.

Common values:
- `static`: Default positioning in the normal document flow.
- `relative`: Positions an element relative to its normal position.
- `absolute`: Positions an element relative to its nearest positioned ancestor, or the initial containing block if none exists.
- `fixed`: Positions an element relative to the viewport.
- `sticky`: Allows an element to behave normally until a scroll threshold is reached, then stick within its containing block.

**Project usage:** The layout uses normal document flow and inline-block elements; positioning properties such as `absolute` and `fixed` are not required.

### C. CSS Overflow
The `overflow` property controls what happens when content does not fit inside an element's box.

Common values:
- `visible`: Content can extend outside the element; this is the default.
- `hidden`: Clips overflowing content.
- `scroll`: Provides scrolling for overflowing content.
- `auto`: Adds scrolling when necessary.

**Project usage:** The hero section is sized using viewport units. The layout should be adjusted to fit the viewport rather than relying on `overflow: hidden` to conceal unwanted scrolling.

### D. CSS Float
The `float` property moves an element to the left or right, allowing surrounding content to flow around it.

Common values:
- `float: left`: Moves the element to the left.
- `float: right`: Moves the element to the right.
- `float: none`: Removes floating behavior.

**Project usage:** Float is not used in the current layout because `display: inline-block` is used to arrange the hero content and navigation elements.

### E. CSS Clear
The `clear` property controls whether an element can appear beside floated elements.

Common values:
- `clear: left`: Prevents the element from appearing beside left-floated elements.
- `clear: right`: Prevents the element from appearing beside right-floated elements.
- `clear: both`: Prevents the element from appearing beside floats on either side.
- `clear: none`: Allows normal placement beside floats.

**Project usage:** Clear is not required because the project does not use the float property.

### F. CSS Hover Effects
The `:hover` pseudo-class applies styles when the pointer is over an element.

**Project usage:** Navigation links change color on hover, and the booking button changes its background color when hovered.

## 4. Conclusion
This project demonstrates the use of HTML, CSS layout techniques, viewport units, the box model, typography, and hover effects to create a laundry services hero section. It also documents important CSS concepts such as display, positioning, overflow, float, and clear for further learning.
