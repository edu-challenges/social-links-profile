# Frontend Mentor - Social links profile solution

This is my solution to the [Social links profile challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/social-links-profile-UG32l9m6dQ).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [Key decisions](#key-decisions)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
  - [AI collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- See hover and focus states for all interactive elements on the page

### Links

- Solution URL: https://github.com/edu-challenges/social-links-profile
- Live Site URL: https://edu-challenges.github.io/social-links-profile/

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow
- Media query for desktop adjustments

### Key decisions

- Semantic structure using main, article, header, nav, and a single list of links.
- Social navigation with an accessible name via aria-label.
- Full-width link buttons within their container for consistent alignment.
- Custom keyboard focus with outline and outline-offset.
- Width controlled at card level (not per link) for cleaner responsive behavior.

### What I learned

- Practical difference between p and span: p for standalone content blocks, span for inline text fragments.
- first-of-type targets the first sibling of that type, not the first element globally in the component.
- max-width sets an upper bound, but does not force growth; desktop growth needs width in the breakpoint.
- Card padding directly affects the visual width of 100% links because of border-box sizing.

Example of the interaction states approach:

```css
a:hover {
  color: var(--grey-800);
  background-color: var(--green);
}

a:focus-visible {
  color: var(--grey-800);
  background-color: var(--green);
  outline: 2px solid var(--white);
  outline-offset: 2px;
}
```

### Useful resources

- [Frontend Mentor style guide](./style-guide.md) - Color, typography, and layout context used during implementation.
- [MDN: :focus-visible](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-visible) - Helped implement accessible keyboard focus styles.
- [MDN: width and max-width](https://developer.mozilla.org/en-US/docs/Web/CSS/max-width) - Clarified responsive sizing behavior.

### AI collaboration

I used GitHub Copilot to support:

- Semantic HTML structure review.
- Accessibility decisions (aria-label, focus-visible, outline behavior).
- Responsive debugging (width vs max-width, specificity, and cascade).
- Layout strategy tuning so links scale correctly with card width.

AI was used as a review and learning assistant, not as a replacement for implementation.

## Author

- GitHub - [Yevestevez](https://github.com/Yevestevez)
- Frontend Mentor - [@Yevestevez](https://www.frontendmentor.io/profile/Yevestevez)
