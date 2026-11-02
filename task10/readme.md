# CSS Transitions and Animations

## 1. Introduction

CSS Transitions and Animations are used to add movement and visual effects to webpage elements.

They make a website more interactive and improve the user experience.

## 2. CSS Transition

A CSS transition allows an element to change its property values smoothly over a specified amount of time.

Transitions generally happen when an element's state changes, such as when the mouse pointer moves over it using the `:hover` pseudo-class.

### Four Main Properties of Transition

The `transition` property consists of four important components:

1. **Transition Property**
2. **Transition Duration**
3. **Transition Timing Function**
4. **Transition Delay**

### A. Transition Property

Specifies which CSS property should have a transition effect.

Example:

```css
button {
    transition-property: background-color;
}
```

Here, only the background color will transition smoothly.

We can also use `all` to apply the transition to all changing properties.

### B. Transition Duration

Specifies how much time the transition takes to complete.

Example:

```css
button {
    transition-duration: 0.5s;
}
```

Here, the transition takes 0.5 seconds to complete.

### C. Transition Timing Function

Controls the speed of the transition at different points during its execution.

Common values:

- `ease` – Starts slowly, speeds up, and ends slowly.
- `linear` – Maintains a constant speed.
- `ease-in` – Starts slowly and speeds up.
- `ease-out` – Starts quickly and slows down.
- `ease-in-out` – Starts and ends slowly.

Example:

```css
button {
    transition-timing-function: ease-in-out;
}
```

### D. Transition Delay

Specifies how long the browser waits before starting the transition.

Example:

```css
button {
    transition-delay: 0.2s;
}
```

Here, the transition starts after a delay of 0.2 seconds.

### Complete Transition Example

```css
button {
    background-color: blue;
    transition: background-color 0.5s ease-in-out 0.2s;
}

button:hover {
    background-color: green;
}
```

In this example:

- `background-color` – Transition property.
- `0.5s` – Duration.
- `ease-in-out` – Timing function.
- `0.2s` – Delay.

When the mouse pointer moves over the button, its background color changes smoothly after the specified delay.

---

## 3. CSS Animation

CSS Animation allows an element to change its styles through multiple stages without requiring the user to hover over or interact with it.

Animations are created using the `@keyframes` rule.

### A. @keyframes

The `@keyframes` rule defines the different stages of an animation.

Example:

```css
@keyframes move {
    0% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-20px);
    }

    100% {
        transform: translateY(0);
    }
}
```

Here:
- `0%` represents the beginning of the animation.
- `50%` represents the middle of the animation.
- `100%` represents the end of the animation.

The element moves upwards and then returns to its original position.

### B. Animation Properties

Some important animation properties are:

- `animation-name` – Specifies the name of the animation.
- `animation-duration` – Specifies how long one animation cycle takes.
- `animation-timing-function` – Controls the speed of the animation.
- `animation-delay` – Specifies when the animation should start.
- `animation-iteration-count` – Specifies how many times the animation repeats.
- `animation-direction` – Specifies the direction in which the animation plays.

### Applying an Animation

```css
.image {
    animation: move 3s ease-in-out 0s infinite;
}
```

Explanation:

- `move` – Name of the animation.
- `3s` – Duration of one cycle.
- `ease-in-out` – Timing function.
- `0s` – Delay.
- `infinite` – Repeats continuously.

---

## 4. Difference Between Transition and Animation

| CSS Transition | CSS Animation |
|---|---|
| Usually requires a change in state to start. | Can start automatically when the page loads. |
| Commonly used with `:hover`, `:focus`, etc. | Uses `@keyframes` to define animation stages. |
| Transitions between two property states. | Can have multiple stages of movement or style changes. |
| Does not repeat automatically. | Can repeat using `animation-iteration-count`. |
| Used for simple interactive effects. | Used for continuous and complex effects. |

### Example of the Difference

**Transition:**

```css
button {
    transition: transform 0.3s ease;
}

button:hover {
    transform: scale(1.1);
}
```

The button increases in size only when the mouse pointer hovers over it.

**Animation:**

```css
@keyframes float {
    0% {
        transform: translateY(0);
    }

    50% {
        transform: translateY(-15px);
    }

    100% {
        transform: translateY(0);
    }
}

.image {
    animation: float 3s ease-in-out infinite;
}
```

The image continuously moves up and down without requiring any mouse interaction.

---

## 5. Conclusion

CSS Transitions and Animations help make webpages more interactive and visually appealing.

- Transitions are useful for smooth changes when an element's state changes, such as hovering over a button.
- Animations are useful for continuous movements and effects that can run automatically.
- `@keyframes` defines the stages of an animation.
- Both transitions and animations can use CSS transform properties such as `scale()`, `rotate()`, and `translate()`.

Understanding these concepts helps create engaging and dynamic web interfaces.
