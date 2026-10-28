# Laundry Services – Hamburger Menu for Mobile

## 1. Project Description
This project extends the Laundry Services website by adding a hamburger menu for mobile screens. The menu allows users to access the navigation links on smaller devices while keeping the desktop navigation layout unchanged.

## 2. Features
- Responsive navigation bar.
- Logo and username displayed on mobile screens.
- Hamburger menu icon visible only on mobile screens.
- Navigation links hidden by default on mobile.
- Menu displayed when the hamburger button receives focus.
- Black menu panel with white navigation links.
- Hover effects on menu links.
- Existing laundry services hero section retained.

## 3. Technologies Used
- HTML5
- CSS3

## 4. CSS Concepts Used

### A. CSS Media Queries
Media queries apply different styles depending on the viewport size.

Example:
```css
@media (max-width: 600px) {
    .nav-links {
        display: none;
    }
}
```

In this project, media queries hide the regular navigation links and display the hamburger menu on mobile screens.

### B. CSS Display Property
The `display` property controls how an element appears in the layout.

- `display: none` hides an element.
- `display: block` displays an element as a block.
- `display: flex` enables Flexbox layout.

In this project, the hamburger menu is hidden by default and displayed on mobile screens. The menu list is initially hidden and shown when the button receives focus.

### C. CSS Positioning
The `position` property controls how an element is positioned.

- `static`: Default positioning.
- `relative`: Positions an element relative to its normal position.
- `absolute`: Positions an element relative to its nearest positioned ancestor.
- `fixed`: Positions an element relative to the viewport.

In this project, `position: fixed` allows the mobile menu panel to cover the screen from the right side.

### D. CSS Focus Pseudo-Class
The `:focus` pseudo-class applies styles when an element receives focus, such as when a user clicks a button or navigates to it using the keyboard.

Example:
```css
.menu-btn:focus + .menu-list {
    display: block;
}
```

Here, the adjacent sibling selector (`+`) selects the menu list immediately following the focused hamburger button. This displays the menu without using JavaScript.

### E. CSS Selectors
The project uses:
- Class selectors, such as `.menu-btn` and `.menu-list`.
- Descendant selectors, such as `.menu-list a`.
- Adjacent sibling selector (`+`) to show the menu when the button receives focus.
- The `:hover` pseudo-class to change the appearance of links when the pointer is over them.

### F. Flexbox
Flexbox is used to arrange the navbar elements and align the logo, username, and hamburger icon.

Important properties include:
- `display: flex`
- `justify-content`
- `align-items`


