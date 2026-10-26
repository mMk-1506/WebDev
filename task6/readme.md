# Laundry Mart Login Page

## 1. Project Description
This project involves creating a login page for a Laundry Mart web application using HTML and CSS. The page has a split layout, with a laundry-related image on the left and a login form on the right. The form includes email and password fields, a login button, a forgot password link, and a registration link.

## 2. Features
- Split-screen login page layout.
- Laundry-themed image on the left section.
- Login form with email and password input fields.
- Forgot Password and Register Now links.
- Styled login button with a hover effect.
- Clean design with blue and white colors.

## 3. Technologies Used
- HTML5
- CSS3

## 4. CSS Concepts Learned

### A. Flexbox
Flexbox is a CSS layout method used to arrange elements along a row or column.

Important properties:
- `display: flex` — enables Flexbox.
- `justify-content` — aligns items along the main axis.
- `align-items` — aligns items along the cross axis.
- `flex-direction` — sets the direction of the items.
- `gap` — adds space between items.

**Project usage:** Flexbox is used to arrange the image section and login form side by side and to organize the content inside the form section.

### B. CSS Grid
CSS Grid is a layout system used to arrange elements into rows and columns.

Important properties:
- `display: grid` — enables Grid layout.
- `grid-template-columns` — defines the columns.
- `grid-template-rows` — defines the rows.
- `gap` — creates spacing between rows and columns.
- `place-items` — aligns items within their grid areas.

**Learning note:** Grid is useful for layouts that need control over both rows and columns. The current login page uses Flexbox for its main layout, while Grid is a concept learned alongside this project.

### C. Grid Positioning
Grid positioning controls where elements appear within a CSS Grid container.

Important properties:
- `grid-column` — specifies the columns an item occupies.
- `grid-row` — specifies the rows an item occupies.
- `grid-area` — assigns an item to a named area or specifies its grid placement.
- `grid-template-areas` — defines named areas in the grid layout.

**Learning note:** These properties can be used to place elements in specific rows, columns, or named areas when building layouts with CSS Grid.

### D. CSS Box Model
The box model describes the space occupied by an element.

Its components are:
- Content
- Padding
- Border
- Margin

**Project usage:** `box-sizing: border-box` helps keep element dimensions predictable by including padding and borders in the declared width and height.
