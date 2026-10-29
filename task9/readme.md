# CSS Laundry Services Button Interactive (Transforms)

## 1. Introduction

In this task, we add a hover effect to the **"Book a service today!"** button in the Laundry Services hero section using CSS transforms.

When the user moves the mouse over the button, its size increases and it tilts slightly. This makes the website more interactive and visually appealing.

## 2. What is CSS Transform?

The CSS `transform` property allows us to change the appearance or position of an element without changing the normal document flow.

CSS provides different transform functions, including:

- `scale()`
- `rotate()`
- `translate()`
- `skew()`

## 3. Transform Functions

### A. Scale

The `scale()` function increases or decreases the size of an element.

**Example:**

```css
button:hover {
    transform: scale(1.1);
}
```

- `scale(1.1)` increases the size by approximately 10%.
- `scale(0.8)` reduces the size to 80% of its original size.
- `scale(1)` keeps the original size.

### B. Rotate

The `rotate()` function rotates an element by a specified angle.

**Example:**

```css
button:hover {
    transform: rotate(-5deg);
}
```

- `rotate(10deg)` rotates the element clockwise.
- `rotate(-5deg)` rotates the element counterclockwise.
- `rotate(0deg)` keeps the element unrotated.

### C. Translate

The `translate()` function moves an element horizontally, vertically, or in both directions.

**Example:**

```css
button:hover {
    transform: translate(10px, -5px);
}
```

- The first value moves the element horizontally.
- The second value moves the element vertically.
- Positive horizontal values move it right, while negative values move it left.
- Positive vertical values move it down, while negative values move it up.

### D. Skew

The `skew()` function slants an element along the horizontal or vertical axis.

**Example:**

```css
button:hover {
    transform: skew(10deg, 5deg);
}
```

- The first value controls horizontal skew.
- The second value controls vertical skew.
- Positive and negative angles create different slant directions.

## 4. Hover Effect Used in This Task

The following CSS is used to increase the button's size and tilt it when the user hovers over it.

```css
.book-btn {
    transition: transform 0.3s ease;
}

.book-btn:hover {
    transform: scale(1.1) rotate(-5deg);
}
```

### Explanation

- `.book-btn` selects the button using its class name.
- `transition: transform 0.3s ease` makes the transformation smooth over 0.3 seconds.
- `.book-btn:hover` applies the styles when the mouse pointer is over the button.
- `scale(1.1)` increases the button's size.
- `rotate(-5deg)` tilts the button counterclockwise.

Multiple transform functions can be combined in a single `transform` property.

