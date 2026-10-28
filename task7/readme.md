# Laundry Services – Responsive Web Design

## 1. Project Description
This project focuses on making the Laundry Services website responsive using HTML and CSS. The existing hero section is modified to work properly on desktop, tablet, and mobile screens using CSS media queries.

## 2. Features
- Navigation bar with Logo, Home, Services, About Us, Contact Us, and Username.
- Hero section with a heading, description, and booking button.
- Laundry-related image displayed alongside the text on desktop.
- Responsive navigation and hero section for different screen sizes.
- Smaller fonts and images on tablet screens.
- Navigation links hidden on mobile screens, keeping the logo and username visible.
- Hero content arranged vertically on mobile screens.

## 3. Technologies Used
- HTML5
- CSS3

## 4. Main Concept: CSS Media Queries

Media queries allow CSS styles to change according to screen size and other device characteristics. They are commonly used to create responsive websites.

### Syntax

```css
@media (max-width: 600px) {
    .nav-links {
        display: none;
    }
}
```

In this example, the navigation links are hidden when the viewport width is 600px or less.

### Media Queries Implemented

**A. Tablet View**

```css
@media (min-width: 601px) and (max-width: 1024px) {
    .hero-left h1 {
        font-size: 2rem;
    }
}
```

- Reduces the heading size for tablet screens.
- Adjusts navigation spacing and font sizes.
- Reduces the image height.
- Keeps the text and image side by side.

**B. Mobile View**

```css
@media (max-width: 600px) {
    .nav-links {
        display: none;
    }

    .hero {
        flex-direction: column;
    }

    .hero-left,
    .hero-right {
        width: 100%;
    }
}
```

- Hides the navigation links on mobile screens.
- Keeps the logo and username visible.
- Places the hero text above the image.
- Adjusts font sizes, padding, and image dimensions.


## 8. Conclusion
This project demonstrates how CSS media queries can make a webpage responsive across different screen sizes. By adjusting font sizes, image dimensions, navigation visibility, and layout direction, the Laundry Services website provides a more suitable viewing experience on desktops, tablets, and mobile devices.
