
# Learning from the Project

## Project Overview

This project was created to build a landing page for promoting Langley tourism. The page features a hero image at the top, followed by a section with three columns, and finally a section combining an image alongside descriptive text.

## General Styling

- Remove default margin and padding from the body and div elements to avoid unwanted spacing:
  ```css
  body {
    margin: 0;
    padding: 0;
  }
  ```
- Use negative `margin-top` on divs to adjust vertical positioning as needed.

## Background Image Styling

- To make a background image stretch to fully cover the div without repeating:
  ```css
  background-image: url(images/newbanner.png);
  background-repeat: no-repeat;
  background-position: center;
  background-size: 100% 100%; /* stretches image to fill entire div */
  ```
- Note: Using `background-size: cover;` is an alternative that covers the div while maintaining aspect ratio but can crop edges.

## Responsive Flexbox Layout

- Use Flexbox for creating columns inside a parent container:
  ```css
  .places {
    display: flex;
    flex-direction: row; /* Default: columns side-by-side */
  }
  ```
- Add responsive behavior with media queries so columns stack vertically on smaller screens:
  ```css
  @media (max-width: 600px) {
    .places {
      flex-direction: column;
    }
  }
  ```
- Design column widths for common device breakpoints:
  - Mobile: 480px width
  - Tablets: 767px width

## Padding and Non-overlapping Items

- Add padding inside child divs to prevent overlap when flexbox columns wrap or stack:
  ```css
  .places > div {
    padding: 10px;
  }
  ```

## Responsive Div Width

- Make divs responsive by setting their width to the smaller of 90% of the screen or 400px:
  ```css
  width: min(90%, 400px);
  ```

## Additional CSS Learnings

- Learned about `:hover`, `transform`, and `transition` properties to create interactive and animated effects on elements.

***

This README captures the purpose, layout, and styling techniques used in the project to promote Langley tourism effectively, using responsive web design principles and visually engaging components.

[1](https://forgeandsmith.com/case-studies/tourism-langley/)
[2](https://www.tourism-langley.ca/wp-content/uploads/2023/12/TLA-2024-Tactical-Plan-Final.pdf)
[3](https://www.ldfp.org/explore)
[4](https://www.langleycity.ca/community-culture/about-langley-city)
[5](https://adventureawaits.ca/things-to-do-in-langley-bc/)
[6](https://www.freepik.com/free-photos-vectors/langley-city-canada-map-designs/24)
[7](https://www.instagram.com/discoverlangleycity/?hl=en)
[8](https://www.discoverlangleycity.com)
[9](https://www.tol.ca/en/connect/maps.aspx)
[10](https://scoutmagazine.ca/places/tourism-langley/)
